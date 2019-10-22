<template>
    <div class="cashless-section">
        <div class="container stars">
          <h2>Join JuanCash towards a cashless Philippines</h2>
          <g-image src="~/assets/images/homepage/section-img-cashless.png" />
        </div>
      </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.cashless-section {
    background-color: $jcdarkblue;
    height: 460px;
    margin-top: 100px;

    .stars {
      height: 460px;

      h2 {
        text-align: center;
        padding-top: 50px;
        color: white;
        font-size: 34px;
      }

      img {
        margin-top: -115px;
      }
    }
  }
</style>