<template>
  <div class="virtual-currencies-section">
    <div class="container virtual-currencies-wrapper">
      <div class="virtual-currencies-left">
        <h2>Virtual Currencies</h2>
        <p>Allows quick buying, selling, exchange of cryptocurrencies and assures the security of crypto assets. Committed to provide secure, transparent and professional digital currency trading services for users worldwide.</p>
        <button class="btn-large">
          Learn More
          <g-image src="~/assets/images/homepage/button-ico-more.png" />
        </button>
      </div>
      <div class="virtual-currencies-right">
        <g-image src="~/assets/images/homepage/section-img-home-vce.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.virtual-currencies-section {
  .virtual-currencies-wrapper {
    margin-top: 200px;
    display: flex;
    justify-content: space-evenly;
    color: black;
    padding: 0 80px;

    p {
      margin-bottom: 20px;
    }
  }
}
</style>