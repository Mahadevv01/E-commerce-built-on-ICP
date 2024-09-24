<script>
  // No need for imports in Svelte, CSS will be scoped within the component
</script>

<style>
  .bannerChild {
    position: absolute;
    top: -360px;
    left: 776.67px;
    border-radius: 99px;
    background-color: #fceed5;
    width: 782.3px;
    height: 635px;
    transform: rotate(25.2deg);
    transform-origin: 0 0;
  }

  .bannerItem {
    position: absolute;
    top: 28.72px;
    left: 41.49px;
    border-radius: 99px;
    background-color: #002a48;
    width: 787.5px;
    height: 787.5px;
    transform: rotate(28.2deg);
    transform-origin: 0 0;
  }

  .everyoneInBizz {
    align-self: stretch;
    position: relative;
    line-height: 68px;
    text-transform: capitalize;
    font-weight: 900;
  }

  .moreShoppingFun {
    align-self: stretch;
    position: relative;
    font-size: 46px;
    line-height: 60px;
    text-transform: capitalize;
    color: #002a48;
  }

  .havingEasySelling {
    width: 394px;
    position: relative;
    font-size: 12px;
    line-height: 18px;
    font-weight: 500;
    color: #242b33;
    text-align: right;
    display: inline-block;
  }

  .everyoneInBizzParent {
    position: absolute;
    top: 64px;
    left: 688px;
    width: 472px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 2px;
    font-size: 52px;
  }

  .clickHere {
    position: relative;
    line-height: 24px;
    font-weight: 500;
  }

  .buttonL {
    position: absolute;
    top: 274px;
    left: 945px;
    border-radius: 57px;
    background-color: #003459;
    width: 163px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: 14px 28px 10px;
    box-sizing: border-box;
    color: #fdfdfd;
  }

  .buttonL1 {
    position: absolute;
    top: 274px;
    left: 764px;
    border-radius: 57px;
    border: 1.5px solid #003459;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: 14px 28px 10px;
  }

  .image25Icon {
    position: absolute;
    top: -83px;
    left: 82px;
    width: 430px;
    height: 440px;
    object-fit: cover;
  }

  .banner {
    width: 100%;
    position: relative;
    border-radius: 20px;
    background-color: #003459;
    height: 378px;
    overflow: hidden;
    text-align: left;
    font-size: 16px;
    color: #003459;
    font-family: Poppins;
    margin: 28px 113px;
  }
</style>

<div class="banner">
  <div class="bannerChild"></div>
  <div class="bannerItem"></div>
  <div class="everyoneInBizzParent">
    <div class="everyoneInBizz">Everyone in bizz</div>
    <b class="moreShoppingFun">more shopping fun!</b>
    <div class="havingEasySelling">
      Having easy selling and buying means you have more joy, a new experience, and be a happy person who will always be within reach of all your needs!
    </div>
  </div>
  <div class="buttonL">
    <div class="clickHere">Explore Now</div>
  </div>
  <div class="buttonL1">
    <div class="clickHere">Sell in Mauzo</div>
  </div>
  <img class="image25Icon" alt="Section" src="/images/image-25.png" />
</div>
