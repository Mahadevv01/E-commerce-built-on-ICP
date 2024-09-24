<script>
    // Any props or state management for the banner can go here
  </script>
  
  <style>
    .herroBannerChild {
        position: absolute;
        top: 268px;
        left: 699.22px;
        border-radius: 99px;
        background-color: #003459;
        width: 635px;
        height: 635px;
        transform:  rotate(9.3deg);
        transform-origin: 0 0;
    }
    .herroBannerItem {
        position: absolute;
        top: 180px;
        left: 865.67px;
        border-radius: 99px;
        background-color: #f7dba7;
        width: 635px;
        height: 635px;
        transform:  rotate(25.2deg);
        transform-origin: 0 0;
    }
    .herroBannerInner {
        position: absolute;
        top: 564px;
        left: 438.33px;
        border-radius: 99px;
        background-color: #f7dba7;
        width: 635px;
        height: 635px;
        transform:  rotate(56.5deg);
        transform-origin: 0 0;
        opacity: 0.4;
    }
    .rectangleDiv {
        position: absolute;
        top: -697px;
        left: -64.33px;
        border-radius: 99px;
        background-color: #f7dba7;
        width: 635px;
        height: 635px;
        transform:  rotate(25.2deg);
        transform-origin: 0 0;
    }
    .herroBannerChild1 {
        position: absolute;
        top: 163px;
        left: 140.6px;
        border-radius: 20px;
        background-color: #f7dba7;
        width: 67.1px;
        height: 67.1px;
        transform:  rotate(25.2deg);
        transform-origin: 0 0;
    }
    .herroBannerChild2 {
        position: absolute;
        top: 148px;
        left: 762.19px;
        border-radius: 4px;
        background-color: #f7dba7;
        width: 14.6px;
        height: 14.6px;
        transform:  rotate(20.8deg);
        transform-origin: 0 0;
    }
    .herroBannerChild3 {
        position: absolute;
        top: 210.68px;
        left: 728px;
        border-radius: 9px;
        background-color: #f7dba7;
        width: 27.5px;
        height: 27.5px;
        transform:  rotate(-22.9deg);
        transform-origin: 0 0;
    }
    .herroBannerChild4 {
        position: absolute;
        top: 223.64px;
        left: 727px;
        border-radius: 6px;
        background-color: #002a48;
        width: 21.5px;
        height: 21.5px;
        transform:  rotate(-43deg);
        transform-origin: 0 0;
    }
    .mauzoShopping {
        position: absolute;
        top: 0px;
        left: 0px;
        line-height: 68px;
        text-transform: capitalize;
        font-weight: 900;
    }
    .moreShoppingFun {
        position: absolute;
        top: 72px;
        left: 0px;
        font-size: 46px;
        line-height: 60px;
        text-transform: capitalize;
    }
    .havingEasySelling {
        position: absolute;
        top: 156px;
        left: 0px;
        font-size: 12px;
        line-height: 18px;
        font-weight: 500;
        color: #242b33;
        display: inline-block;
        width: 480px;
    }
    .clickHere {
        position: relative;
        line-height: 24px;
        font-weight: 500;
    }
    .buttonL {
        position: absolute;
        top: 0px;
        left: 181px;
        border-radius: 57px;
        background-color: #003459;
        width: 163px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        padding: 14px 28px 10px;
        box-sizing: border-box;
    }
    .buttonL1 {
        position: absolute;
        top: 0px;
        left: 0px;
        border-radius: 57px;
        border: 1.5px solid #003459;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        padding: 14px 28px 10px;
        color: #003459;
    }
    .buttonLParent {
        position: absolute;
        top: 262px;
        left: 0px;
        width: 344px;
        height: 48px;
        font-size: 16px;
        color: #fdfdfd;
    }
    .description {
        position: absolute;
        top: 180px;
        left: 130px;
        width: 751px;
        height: 310px;
    }
    .image24Icon {
        position: absolute;
        top: 52px;
        left: 856px;
        width: 391px;
        height: 600px;
        object-fit: cover;
    }
    .image25Icon {
        position: absolute;
        top: 360px;
        left: 542px;
        width: 350px;
        height: 350px;
        object-fit: cover;
    }
    .herroBanner {
        width: 100%;
        position: relative;
        border-radius: 0px 0px 40px 40px;
        background: linear-gradient(102.87deg, #fceed5 6.17%, #fceed5 75.14%, #ffe7ba);
        height: 695px;
        overflow: hidden;
        text-align: left;
        font-size: 60px;
        color: #002a48;
        font-family: Poppins;
    }



  </style>
  
  <div class="herroBanner">
    <div class="herroBannerChild"></div>
    <div class="herroBannerItem"></div>
    <div class="herroBannerInner"></div>
    <div class="rectangleDiv"></div>
    <div class="herroBannerChild1"></div>
    <div class="herroBannerChild2"></div>
    <div class="herroBannerChild3"></div>
    <div class="herroBannerChild4"></div>
    <div class="description">
      <div class="mauzoShopping">{ `Mauzo Shopping` }</div>
      <b class="moreShoppingFun">more shopping fun!</b>
      <div class="havingEasySelling">Having easy selling and buying means you have more joy, a new experience, and be a happy person who will always be within reach of all your needs!</div>
      <div class="buttonLParent">
        <div class="buttonL">
            <div class="clickHere"> Explore Now </div>
        </div>
        <div class="buttonL1">
            <div class="clickHere"> Sell In Mauzo </div>
        </div>
      </div>
    </div>
    
    <img class="image24Icon" src="/images/image-24.png" alt="Shopping Image" />
    <img class="image25Icon" src="/images/image-25.png" />
  </div>
  