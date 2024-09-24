<script>
    let logos = [
        "images/holdersImages/image-4.png",
        "images/holdersImages/image-9.png",
        "images/holdersImages/image-10.png",
        "images/holdersImages/image-11.png"
    ];

    let animationPaused = false;

    // Pause carousel on hover
    const stopCarousel = () => {
        animationPaused = true;
    };

    // Resume carousel on mouse leave
    const startCarousel = () => {
        animationPaused = false;
    };
</script>

<style>
    .proudToBe {
        position: relative;
        line-height: 31px;
        font-weight: 500;
    }

    .mauzoBusiness {
        position: relative;
        font-size: 24px;
        line-height: 36px;
        text-transform: capitalize;
        color: #003459;
    }

    .proudToBePartOfParent {
        display: flex;
        flex-direction: row;
        align-items: flex-end;
        justify-content: flex-start;
        gap: 8px;
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
        cursor: pointer;
    }

    .frameGroup {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        width: 100%;
    }

    .imageWrapper {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 10px;
        cursor: pointer;
    }

    .imageIcon {
        width: 100px;
        height: auto;
        object-fit: cover;
        transition: transform 0.3s;
    }

    .imageIcon:hover {
        transform: scale(1.05);
    }

    .frameParent {
        width: 100%;
        padding: 40px 130px;
        box-sizing: border-box;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        gap: 15px;
        text-align: left;
        font-size: 16px;
        font-family: Poppins, sans-serif;
    }

    .frameContainer {
        width: 100%;
        overflow: hidden;
        position: relative;
    }

    .carousel {
        display: flex;
        flex-direction: row;
        gap: 20px;
        animation: scroll 20s linear infinite;
        animation-play-state: running;
    }

    /* Pausing the animation when the user hovers */
    .carousel.paused {
        animation-play-state: paused;
    }

    .imageWrapper {
        flex: 0 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .imageIcon {
        width: 100px;
        height: auto;
        object-fit: cover;
        transition: transform 0.3s;
    }

    .imageIcon:hover {
        transform: scale(1.05);
    }

    /* Smooth scrolling effect, looping back to the start */
    @keyframes scroll {
        from {
            transform: translateX(0);
        }
        to {
            transform: translateX(-50%);
        }
    }

</style>

<div class="frameParent">
    <div class="frameGroup">
        <div class="proudToBePartOfParent">
            <div class="proudToBe">Proud to be part of</div>
            <b class="mauzoBusiness">Mauzo Business</b>
        </div>
        <div class="buttonM">
            <div class="clickHere">View all our sellers</div>
            <img class="arrowChevronRightMd" alt="" src="icons/arrow-chevron-right-md.svg" />
        </div>
    </div>

    <!-- Carousel Container -->
    <div
        class="frameContainer"
        role="button"
        tabindex="0"
        on:mouseover={stopCarousel}
        on:mouseleave={startCarousel}
        on:focus={stopCarousel}
    >
        <!-- Carousel Wrapper -->
        <div class="carousel {animationPaused ? 'paused' : ''}">
            {#each logos.concat(logos) as logo}
                <div class="imageWrapper">
                    <img class="imageIcon" src={logo} alt="logo" />
                </div>
            {/each}
        </div>
    </div>
</div>
