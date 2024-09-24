<script>
  import Header from '../components/Header.svelte';
  import Banner from '../components/Banner.svelte';
  import ProductCard from '../components/ProductCard.svelte';
  import Footer from '../components/Footer.svelte';
  import SectionBurner from '../components/SectionBurner.svelte';
  import Logocarousel from '../components/Logocarousel.svelte';

  

  let products = [
    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals. Very good at heavy weight tasks. The powerful app with touch screen and good battery life',
      price: '6.900.000',
      image: 'images/product-card-image-2.png'
    },

    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals. Perfect Intel chips for AI and ML tasks',
      price: '6.900.000',
      image: '/images/image-25.png'
    },

    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals. Another moment to explore the perfect task of performance. Another moment to explore the perfect task of performance and machine work. Perfection of this age',
      price: '6.900.000',
      image: 'images/product-card-image-2.png'
    },
    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals. Another moment to explore the perfect task of performance. Another moment to explore the perfect task of performance and machine work. Perfection of this age',
      price: '6.900.000',
      image: 'images/product-card-image-2.png'
    },
    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals. Another moment to explore the perfect task of performance. Another moment to explore the perfect task of performance and machine work. Perfection of this age',
      price: '6.900.000',
      image: 'images/product-card-image-2.png'
    },
    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals. Another moment to explore the perfect task of performance. Another moment to explore the perfect task of performance and machine work. Perfection of this age',
      price: '6.900.000',
      image: 'images/product-card-image-2.png'
    },

    {
      name: 'HP8420 - Hp Laptop',
      description: 'A powerful laptop for professionals.',
      price: '6.900.000',
      image: '/images/image-24.png'
    },
    // Add more products
  ];
</script>

<style>
  /* Add any global or layout styles */

    .whatsNew {
      position: relative;
      line-height: 24px;
      font-weight: 500;
    }

    .products {
      position: relative;
      font-size: 24px;
      line-height: 36px;
      text-transform: capitalize;
      color: #003459;
    }

    .whatsNewParent {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: 2px;
    }

    .clickHere {
      position: relative;
      line-height: 20px;
      font-weight: 500;
    }

    .arrowChevronRightMd {
      width: 20px;
      position: relative;
      height: 20px;
      overflow: hidden;
      flex-shrink: 0;
    }

    .buttonM {
      border-radius: 57px;
      border: 1.5px solid #003459;
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: center;
      padding: 12px 28px;
      gap: 8px;
      font-size: 14px;
      color: #003459;
    }

    .productssectionheader {
      width: 100%;
      position: relative;
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-between;
      text-align: left;
      font-size: 16px;
      color: #000;
      font-family: Poppins;
    }
    .productListSection {
      width: 100%;
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 20px 112px;
      box-sizing: border-box;
      gap: 4px;
      text-align: left;
      font-size: 16px;
      color: #000;
      font-family: Poppins;
    }

    .whatsNewParent {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: 2px;
    }

    .productsListsDesktop {
      width: 100%;
      position: relative;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: center;
      flex-wrap: wrap;
      align-content: flex-start;
      gap: 20px;
      text-align: left;
      font-size: 16px;
      color: #00171f;
      font-family: Poppins;
    }

    main{
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin-right: 0;
    }


</style>

<Header />

<main class="mainSection">
  <Banner />
  
  <section class="productListSection">
    <div class="productssectionheader">
      <div class="whatsNewParent">
        <div class="whatsNew">What’s new?</div>
        <b class="products">Products</b>
      </div>
      <div class="buttonM">
        <div class="clickHere">View more</div>
        <img class="arrowChevronRightMd" alt="" src="icons/arrow-chevron-right-md.svg" />
      </div>
    </div>
    <div class="productsListsDesktop">
      {#each products as product}
        <ProductCard {product} />
      {/each}
     </div>
  </section>
  <SectionBurner />
  <Logocarousel />
</main>

<Footer />
