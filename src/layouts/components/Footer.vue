<template>
  <footer class="footer container">
    <div class="zybi-section">
      <a href="http://www.zybitech.com">
        <g-image src="~/assets/images/homepage/footer-logo-zybitech.png" />
      </a>
      <p>8th Floor IMET BPO Tower, Metropolitan Avenue, Roxas Boulevard, Pasay City, Philippines</p>
      <br />
      <p>(028878-0889</p>
      <p>apps@zybitech.com</p>
      <p>info@zybitech.com</p>
      <br />
      <p>&copy; 2019 JuanCash. All rights reserved.</p>
    </div>
    <div class="quick-links">
      <h4>Quick Links</h4>
      <div class="links-container">
        <div class="links-container-left flex-column">
          <g-link to="/business">Business</g-link>
          <g-link to="/merchants">Merchants</g-link>
          <g-link to="/blog">Blog</g-link>
          <g-link to="/promos">Promos</g-link>
          <g-link to="/faq">FAQs</g-link>
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
        <a href="https://www.facebook.com/JuanCashOfficial/">
          <g-image src="~/assets/images/homepage/footer-social-facebook.png" />
        </a>
        <a href="">
          <g-image src="~/assets/images/homepage/footer-social-wechat.png" />
        </a>
        <a href="https://twitter.com/juancash__">
          <g-image src="~/assets/images/homepage/footer-social-twitter.png" />
        </a>
        <a href="https://www.instagram.com/juancashofficial/">
          <g-image src="~/assets/images/homepage/footer-social-instagram.png" />
        </a>
      </div>
    </div>
    <div class="qr-code">
      <g-image src="~/assets/images/homepage/footer-img-qrcode.jpg" />
      <p>Scan to download JuanCash app.</p>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  padding-top: 50px;
  height: 350px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  justify-items: stretch;

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
          text-decoration: none;
        }
      }
    }
  }

  .juancash-section {
    display: flex;
    flex-flow: column;
    align-items: center;
    .social-container {
      img {
        margin-right: 10px;
      }
    }
  }

  .qr-code {
    display: flex;
    flex-flow: column;
    justify-content: flex-start;
    align-items: center;
  }
}
</style>