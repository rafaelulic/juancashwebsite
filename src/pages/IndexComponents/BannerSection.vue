<template>
  <div class="banner-section">
    <div class="container banner-wrapper">
      <div class="banner-left">
        <h1>Your All-in-Juan Financial App</h1>
        <p>Enjoy cashless &amp; hassle-free transactions with your e-wallet partner toward financial convenience!</p>
        <div class="download-images">
          <div class="download-images-left">
            <g-image src="~/assets/images/homepage/btn-ico-app-android.png" />
            <g-image src="~/assets/images/homepage/btn-ico-app-ios.png" />
          </div>
          <div class="download-images-right">
            <g-image src="~/assets/images/homepage/btn-ico-app-qr.png" />
            <p class="scan">Scan to download JuanCash App</p>
          </div>
        </div>
      </div>
      <div class="banner-right">
        <g-image src="~/assets/images/homepage/section-img-banner.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.banner-section {
  background-color: $jcblue;
  height: 500px;

  .banner-wrapper {
    padding: 50px;

    display: flex;
    justify-content: flex-start;

    .banner-left {
      padding-right: 200px;

      .download-images {
        padding-top: 24px;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        
        .scan {
          font-size: 11px;
          text-align: center;
          width: 120px;
          line-height: 12px;
        }
      }
    }
  }
}
</style>
