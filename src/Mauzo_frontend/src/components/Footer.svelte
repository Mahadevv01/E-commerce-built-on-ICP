<script>
  // Import necessary image assets
</script>


<style>
  /* General Styles */
  .footer {
    width: 100%;
    background: linear-gradient(102.87deg, #fceed5 6.17%, #fceed5 75.14%, #ffe7ba);
    padding: 40px;
    box-sizing: border-box;
    border-radius: 40px 40px 0 0;
    font-family: 'Poppins', sans-serif;
  }
  .footnote {
    width: 80%;
    position: relative;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    text-align: center;
    font-size: 14px;
    color: #667479;
    font-family: Poppins;
  }

  .contacting {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 40px;
  }

  .mauzo-all-rights, .terms-of-service {
    font-size: 14px;
    color: #667479;
  }

  .logotext {
    width: 119px;
    overflow: hidden;
    flex-shrink: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
  }

  .appmoto {
    width: 68.3px;
    position: relative;
    height: 17.6px;
  }
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
    width: 68.3px;
    position: relative;
    font-size: 10px;
    line-height: 16px;
    font-weight: 500;
    font-family: Poppins;
    color: #103559;
    text-align: left;
    display: inline-block;
    height: 17.6px;
  }

  .icon {
    width: 24px;
    height: 24px;
  }

  /* Input Styles */
  .input-container {
    display: flex;
    gap: 10px;
  }

  .input {
    padding: 14px;
    border-radius: 8px;
    border: 1px solid #99a2a5;
    flex: 1;
    background-color: #fff;
  }

  .button-l {
    padding: 14px;
    background-color: #003459;
    color: white;
    border-radius: 8px;
    font-weight: 500;
    cursor: pointer;
  }

  /* Contact Section */
  .contact-home {
    display: flex;
    justify-content: space-between;
    width: 100%;
    max-width: 800px;
  }

  .home-parent a {
    color: #00171f;
    text-decoration: none;
    font-size: 16px;
    font-weight: 500;
    margin-right: 40px;
  }

  .social-media img {
    position: relative;
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 60px;
    text-align: left;
    font-size: 16px;
    color: #00171f;
    font-family: Poppins;
  }

  /* Mobile Responsiveness */
  @media (max-width: 768px) {
    .footer {
      padding: 20px;
    }
    .footnote {
        width: 80%;
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        text-align: left;
        font-size: 14px;
        color: #667479;
        font-family: Poppins;
    }

    .logotext {
      font-size: 12px;
      padding: 0;
      margin: 0;
    }

    .mauzo-all-rights, .terms-of-service {
      font-size: 12px;
    }

    .contact-home {
      flex-direction: column;
      align-items: center;
      gap: 20px;
    }

    .input-container {
      flex-direction: column;
      gap: 5px;
    }
  }

  /* Desktop Responsiveness */
  @media (min-width: 768px) {
    .contact-home {
      flex-direction: row;
      justify-content: space-between;
    }

    .input-container {
      flex-direction: row;
    }
  }
</style>


<div class="footer">
  <div class="contacting">
    <div class="contact-home">
      <div class="home-parent">
        <a class="click-here" href="/">Home</a>
        <a class="click-here" href="/category">Category</a>
        <a class="click-here" href="/about">About</a>
        <a class="click-here" href="/contact">Contact</a>
      </div>
      <div class="social-media">
        <a href="" target="_blank" rel="noopener noreferrer">
          <span class="iconify" data-icon="mdi:facebook" data-inline="false"></span>
        </a>
        <a href="" target="_blank" rel="noopener noreferrer">
          <span class="iconify" data-icon="mdi:whatsapp" data-inline="false"></span>
        </a>
        <a href="" target="_blank" rel="noopener noreferrer">
          <span class="iconify" data-icon="mdi:linkedin" data-inline="false"></span>
        </a>
      </div>
    </div>
  </div>
  <div class="footnote">
    <div class="mauzo-all-rights">© 2024 Mauzo. All rights reserved.</div>
    <div class="logotext">
        <img class="imageIcon " src="/Logo.png" alt="Logo" />
      <div class="appmoto">
        <div class="shopForBest">Shop for Best</div>
      </div>
    </div>
    <div class="terms-of-service">Terms of Service | Privacy Policy</div>
  </div>
</div>
