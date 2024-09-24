<script>
    export let product = {};
    let showSeeMore = false;
    
    // Check if description exceeds a certain length
    $: showSeeMore = product.description.length > 100; // Example threshold of 100 characters
</script>

<style>
.productCard {
    position: relative;
    box-shadow: 0px 4px 28px -2px rgba(0, 0, 0, 0.08);
    border-radius: 12px;
    background-color: #fdfdfd;
    width: 270px; 
    height: auto; 
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 8px;
    box-sizing: border-box;
    gap: 8px;
    text-align: left;
    font-size: 16px;
    color: #00171f;
    font-family: Poppins;
}

.productImage {
    width: 100%; /* To ensure image scales with container */
    height: 264px;
    border-radius: 10px;
    object-fit: cover;
}

.productDecriptionAndName {
    display: flex;
    flex-direction: column;
    gap: 4px;
    width: 100%;
}

.productName {
    font-weight: bold;
    font-size: 16px;
    line-height: 1.2;
}

.productDescription {
    font-size: 12px;
    color: #667479;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: wrap;
    display: -webkit-box;
    -webkit-line-clamp: 2; /* Display up to 3 lines of text */
    -webkit-box-orient: vertical;
}

.seeMoreParent {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    font-size: 14px;
    color: #99a2a5;
}

.seeMore {
    cursor: pointer;
    color: blue;
}

.price {
    color: #00171f;
    font-weight: bold;
}

.actionButtons {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    font-size: 14px;
    color: #002a48;
	margin-top: 2px;
}

.frameContainer, .buyWrapper {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 6px 10px;
    border-radius: 8px;
    background-color: #fceed5;
}

.addToCart {
    font-weight: bold;
    margin-left: 4px;
}
</style>

<div class="productCard">
    <img class="productImage" src={product.image} alt={product.name} />
    <div class="productDecriptionAndName">
        <b class="productName">{product.name}</b>
        <p class="productDescription">{product.description}</p>
    </div>
    
    <div class="seeMoreParent">
        {#if showSeeMore}
            <div class="seeMore">See More...</div>
        {/if}
        <div class="price">{product.price} VND</div>
    </div>
    
    <div class="actionButtons">
        <div class="frameContainer">
            <img src="icons/product-card-fi-rr-shopping-cart-add.svg" alt="Add to cart" class="frameIcon" />
            <b class="addToCart">Add to cart</b>
        </div>
        <div class="buyWrapper">
            <b>Buy</b>
        </div>
    </div>
</div>
