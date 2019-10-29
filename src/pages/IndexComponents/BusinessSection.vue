<template>
  <div class="business-section">
    <div class="container business-container">
      <div class="business-section-left">
        <g-image src="~/assets/images/homepage/section-img-home-business.png" />
      </div>
      <div class="business-section-right">
        <h2>JuanCash Business</h2>
        <p>Boost your business by diversifying your payment options via our latest QR technology</p>
        <g-link to="/business" class="btn-large">
          Learn More
          <g-image src="~/assets/images/homepage/button-ico-more.png" />
        </g-link>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style lang="scss" scoped>
.business-section { 
  height: 337px;
  background-color: $jcblue;
  .business-container {
    display: flex;

    h2 {
      color: white;
    }

    .business-section-right {
      display: flex;
      flex-direction: column;
      justify-content: center;

      width: 520px;

      p {
        margin-bottom: 20px;
      }
    }
  }
}
</style>