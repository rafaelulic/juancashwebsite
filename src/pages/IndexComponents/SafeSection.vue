<template>
  <div class="safe-section">
    <div class="container">
      <h2>JuanCash is S.A.F.E.</h2>
      <div class="safe-card-container">
        <div class="card" :key="item" v-for="item of items">
          <div class="card-content">
            <div class="image">
              <g-image :src="item.image" /> />
            </div>
            <div class="text">
              <h3>{{item.title}}</h3>
              <p>{{item.content}}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import image1 from "../../assets/images/homepage/section-img-safe-1secured.png"
export default {
  data: function () {
    return {
      items: [
        {image: "~/assets/images/homepage/section-img-safe-1secured.png", title: 'Secured', content: "Our solution uses the latest QR Technology"},
        {image: "~/assets/images/homepage/section-img-safe-2accepted.png", title: 'Accepted', content: "Use your JuanCash wallet to pay/ fund transfer to over 70+ accredited billers, merchants &amp; store partners."},
        {image: "~/assets/images/homepage/section-img-safe-3fast.png", title: 'Fast', content: "With a few taps on the customer's mobile phone, the transaction is complete."},
        {image: "~/assets/images/homepage/section-img-safe-4easy.png", title: 'Easy', content: "Consumer scans your store's QR code, input amount due, then send. Done!"}
      ]
    }
  }
}
</script>

<style lang='scss' scoped>
.safe-section {
  margin-top: 50px;

  h2 {
    color: $jcblue;
    text-align: center;
    margin-bottom: 50px;
  }

  .safe-card-container {
    .card {
      width: 568px;
      height: 160px;
      border-radius: 8px;
      border: solid 2px #91e1ff;
      padding: 20px;

      .card-content {
        display: flex;

        .text {
          padding-left: 20px;

          h3 {
            color: $jcblue;
          }

          p {
            color: black;
          }
        }
      }
    }
  }
}
</style>