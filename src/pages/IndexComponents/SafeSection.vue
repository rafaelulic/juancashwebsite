<template>
  <div class="safe-section">
    <div class="container">
      <h2>JuanCash is S.A.F.E.</h2>
      <div class="safe-card-container">
        <div class="card" :key="item.index" v-for="item of items">
          <div class="card-content">
            <div class="image">
              <g-image :src="require('../../assets/images/homepage/'+item.image)" />
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
export default {
  data: function() {
    return {
      items: [
        {
          index: 0,
          image: "section-img-safe-1secured.png",
          title: "Secured",
          content: "Our solution uses the latest QR Technology"
        },
        {
          index: 1,
          image: "section-img-safe-2accepted.png",
          title: "Accepted",
          content:
            "Use your JuanCash wallet to pay/ fund transfer to over 70+ accredited billers, merchants & store partners."
        },
        {
          index: 2,
          image: "section-img-safe-3fast.png",
          title: "Fast",
          content:
            "With a few taps on the customer's mobile phone, the transaction is complete."
        },
        {
          index: 3,
          image: "section-img-safe-4easy.png",
          title: "Easy",
          content:
            "Consumer scans your store's QR code, input amount due, then send. Done!"
        }
      ]
    }
  }
}
</script>

<style lang='scss' scoped>
.safe-section {
  margin-top: 50px;

  h2 {
    font-size: 44px;
    text-align: center;
    margin-bottom: 50px;
  }

  .safe-card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

    .card {
      width: 568px;
      height: 160px;
      border-radius: 8px;
      border: solid 2px #91e1ff;
      padding: 20px;
      margin: 10px;

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