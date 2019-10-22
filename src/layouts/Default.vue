<template>
  <div class="layout">
    <header class="header">
      <nav class="navbar container">
        <div class="logo">
          <g-link to="/"><g-image alt="JuanCash Logo" src="~/assets/images/homepage/logo-juancash.png" /></g-link>
        </div>
        
        <div class="nav-link-container">
          <ul class="nav-link-wrapper">
            <li>
              <g-link to="/">Home</g-link>
            </li>
            <li>
              <g-link to="/about">Business</g-link>
            </li>
            <li>
              <g-link to="/business">Merchants</g-link>
            </li>
            <li>
              <g-link>Learn More</g-link>
            </li>
            <li>
              <g-link>Contact Us</g-link>
            </li>
            <li>
              <g-link><g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-facebook.png" /></g-link>
            </li>
            <li>
              <g-link><g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-wechat.png" /></g-link>
            </li>
            <li>
              <g-link><g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-twitter.png" /></g-link>
            <li>
              <g-link><g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-instagram.png" /></g-link>
            </li>
            <li>
              <button class="button">English</button>
              <!-- <g-link><g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-facebook.png" /></g-link> -->
            </li>
          </ul>
        </div>
      </nav>
    </header>
    <slot/>
    <footer class="footer container">
      <div class="zybi-section">
        <g-image src="~/assets/images/homepage/footer-logo-zybitech.png" />

        <p>8th Floor IMET BPO Tower, Metropolitan Avenue, Roxas Boulevard, Pasay City, Philippines</p>

        <p>(028878-0889</p>
        <p>apps@zybitech.com</p>
        <p>info@zybitech.com</p>
        <p>&copy; 2019 JuanCash. All rights reserved.</p>
      </div>
      <div class="quick-links">
        <h4>Quick Links</h4>
        <div class="links-container">
          <div class="links-container-left flex-column">
            <g-link>Business</g-link>
            <g-link>Merchants</g-link>
            <g-link>Blog</g-link>
            <g-link>Promos</g-link>
            <g-link>FAQs</g-link>
          </div>
          <div class="links-container-right flex-column">
            <g-link>Contact Us</g-link>
            <g-link>Terms and Conditions</g-link>
            <g-link>Privacy Policy</g-link>
          </div>
        </div>
      </div>
      <div class="juancash-section">
        <g-image src="~/assets/images/homepage/footer-logo-juancash.png" />
        <h4>Connect with us</h4>
        <div class="social-container">
          <g-image src="~/assets/images/homepage/footer-social-facebook.png" />
          <g-image src="~/assets/images/homepage/footer-social-wechat.png" />
          <g-image src="~/assets/images/homepage/footer-social-twitter.png" />
          <g-image src="~/assets/images/homepage/footer-social-instagram.png" />
        </div>
      </div>
      <div class="qr-code">
        <g-image src="~/assets/images/homepage/footer-img-qrcode.jpg" />
        <p>Scan to download JuanCash app.</p>
      </div>
    </footer>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style lang='scss'>
.header {
  width: 100%;
  background: $jcblue;  
  margin-bottom: 20px;
  height: 525px;
  
  .navbar {
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: flex-start;

    .nav-link-container {
      flex: 1;
      .nav-link-wrapper {
        list-style: none;
        height: 80px;
        margin: 0;

         
        display: flex;
        justify-content: flex-end;        
        align-items: center;
        
        li {
          padding-left: 10px;

          a {
            text-decoration: none;
            color: white;
            text-transform: uppercase;
          }
        }



      }
    }
  }
}

.footer {
  padding-top: 100px;
  height: 350px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  
  h4 {
      font-size: 16px;
      text-transform: uppercase;
      margin-bottom: 20px;
  }

  p {
    font-size: 14px;
  }

  .quick-links {
    .links-container {
      display: flex;

      .links-container-left {
        flex: 1;
      }

      .flex-column {
        display: flex;
        flex-direction: column;

        a {
          color: black;
          margin-bottom: 20px;
        }
      }
    }
  }

  .juancash-section {
    padding-left: 30px;
    .social-container {
      img {
        margin-right: 10px;
      }
    }
  }
}
</style>
