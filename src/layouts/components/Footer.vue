<template>
  <footer class="footer container">
    <div class="zybi-section">
      <g-image src="~/assets/images/homepage/footer-logo-zybitech.png" />

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
    padding-left: 30px;
    .social-container {
      img {
        margin-right: 10px;
      }
    }
  }
}
</style>