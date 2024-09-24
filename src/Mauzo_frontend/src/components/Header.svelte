<script>
    // This script could contain any logic or reactive declarations needed for your header
  </script>
  
  <style>
    
    .imageIcon {
        align-self: stretch;
        position: relative;
        max-width: 100%;
        overflow: hidden;
        height: 28px;
        flex-shrink: 0;
        object-fit: cover;
    }
    .shopForBest {
        position: absolute;
        height: 100%;
        width: 100%;
        top: 0%;
        left: 0%;
        line-height: 16px;
        font-weight: 500;
        display: inline-block;
    }
    .group {
        width: 68.3px;
        position: relative;
        height: 17.6px;
    }
    .frame {
        width: 119px;
        overflow: hidden;
        flex-shrink: 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
    }
    .home {
        position: relative;
        line-height: 24px;
    }
    .homeParent {
        display: flex;
        flex-direction: row;
        align-items: flex-start;
        justify-content: flex-start;
        gap: 48px;
        font-size: 16px;
        color: #003459;
    }
    .frameParent {
        height: 44px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: flex-start;
        gap: 48px;
    }
    .usearchIcon {
        width: 20px;
        position: relative;
        height: 20px;
        overflow: hidden;
        flex-shrink: 0;
    }
    .searchSomethingHere {
        position: relative;
        line-height: 20px;
        font-weight: 500;
    }
    .usearchParent {
        width: 280px;
        border-radius: 46px;
        background-color: #fdfdfd;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: flex-start;
        padding: 12px 20px 12px 16px;
        box-sizing: border-box;
        gap: 12px;
        font-size: 14px;
    }

    .search {
        border-radius: none;
        border: none;
        cursor: auto;
        outline: none; /* Added outline property to remove border when active */
    }

    .buttonL {
        border-radius: 57px;
        background-color: #003459;
        height: 44px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        padding: 14px 28px 10px;
        box-sizing: border-box;
        color: #fdfdfd;
    }
    .frameChild {
        width: 21px;
        position: relative;
        height: 21px;
        overflow: hidden;
        flex-shrink: 0;
    }
    .vnd {
        position: relative;
        line-height: 23px;
        font-weight: 500;
    }
    .frameDiv {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: flex-start;
        gap: 6px;
    }
    .arrowCaretDownSm {
        width: 24px;
        position: relative;
        height: 24px;
        overflow: hidden;
        flex-shrink: 0;
    }
    .frameContainer {
        align-self: stretch;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: flex-end;
        padding: 10px 8px 8px;
        gap: 4px;
        color: #002a48;
    }
    .frameGroup {
        display: flex;
        flex-direction: row;
        align-items: flex-start;
        justify-content: flex-start;
        gap: 14px;
        font-size: 16px;
        color: #99a2a5;
    }
    .headerDesktop {
        width: 100%;
        position: absolute; /* Overlay the header on top of the banner */
        top: 0; /* Position the header at the top of the page */
        left: 0;
        /* position: relative; */
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        padding: 28px 113px;
        box-sizing: border-box;
        text-align: left;
        font-size: 10px;
        color: #103559;
        font-family: Poppins;
        z-index: 10; /* Ensure the header appears above the banner */
        background-color: transparent; /* Make the header background transparent */
    }

  </style>
  <div class="headerDesktop">
    <div class="frame">
        <img class="imageIcon " src="/Logo.png" alt="Logo" />
      <div class="group">
        <div class="shopForBest">Shop for Best</div>
      </div>
    </div>
    <div class="homeParent">
      <b>Home</b>
      <b>Category</b>
      <b>About</b>
      <b>Contact</b>
    </div>
    <div class="frameGroup">
      <div class="usearchParent">
          <input class="search" placeholder="Search something here!" />
          <img src="/icons/u-search.svg" alt="Search" />
      </div>
      <div class="buttonL">
        <b>Join </b>
      </div>
      <div class="frameContainer">
        <div class="frameDiv">
        <img class="frameChild" alt="" src="images/frame.svg" />
        <div class="vnd">VND</div>
        </div>
        <img class="arrowCaretDownSm" alt="" src="icons/arrow-caret-down-sm.svg" />
        </div>
    </div>
  </div>
  