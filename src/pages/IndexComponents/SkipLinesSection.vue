<template>
  <div class="skip-lines-section">
    <div class="container">
      <p class="skip-tagline">Skip The Lines, Pay Your Bills Via JuanCash App!</p>
      <div class="biller-container">
        <g-image src="~/assets/images/homepage/biller-cignal.png" />
        <g-image src="~/assets/images/homepage/biller-skycable.png" />
        <g-image src="~/assets/images/homepage/biller-smart.png" />
        <g-image src="~/assets/images/homepage/biller-globe.png" />
        <g-image src="~/assets/images/homepage/biller-pldt.png" />
        <g-image src="~/assets/images/homepage/biller-meralco.png" />
        <g-image src="~/assets/images/homepage/biller-manila-water.png" />
        <g-image src="~/assets/images/homepage/biller-maynilad.png" />
        <g-image src="~/assets/images/homepage/biller-home-credit.png" />
        <g-image src="~/assets/images/homepage/biller-aeon.png" />
      </div>
      <div class="offer">
        <div class="offer-left">
          <g-image src="~/assets/images/homepage/section-img-home-offer.png" />
        </div>
        <div class="offer-right">
          <h2>Here's What JuanCash Has To Offer</h2>
          <div class="offer-list">
            <g-image src="~/assets/images/homepage/section-home-offer-ico-check.png" />
            <div class="offer-list-group">
              <h3>Payment of Utilities and other Bills</h3>
              <p>Never miss paying bills. JuanCash gives you the ability to pay more than 75 billers, including the major utilities companies.</p>
            </div>
          </div>
          <div class="offer-list">
            <g-image src="~/assets/images/homepage/section-home-offer-ico-check.png" />
            <div class="offer-list-group">
              <h3>Prepaid Load Purchases</h3>
              <p>JuanCash lets you top on prepaid load products from all major telecommunication service providers.</p>
            </div>
          </div>
          <div class="offer-list">
            <g-image src="~/assets/images/homepage/section-home-offer-ico-check.png" />
            <div class="offer-list-group">
              <h3>Cardless Withdrawals</h3>
              <p>Do away with physical cards. Withdraw from ATM machines of our partner institutions without the need from an ATM card.</p>
            </div>
          </div>
          <div class="offer-list">
            <g-image src="~/assets/images/homepage/section-home-offer-ico-check.png" />
            <div class="offer-list-group">
              <h3>WeChat Payment Partner</h3>
              <p>JuanCash is now accredited by WeChat as its payment partner.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
 
<script>
export default {}
</script>

<style lang="scss" scoped>
.skip-lines-section {
    background-image: url("~@/assets/images/homepage/blue-bg.png");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    height: 874px;
    margin-top: -68px;
    padding-top: 220px;

    .skip-tagline {
      font-size: 24px;
      font-weight: bold;
      margin-bottom: 20px;
    }

    .biller-container {
      height: 90px;
      border-radius: 50px;
      background-color: white;
      padding: 0 50px;
      display: flex;
      justify-content: space-around;
      align-items: center;
      width: 800px;
    }

    .offer {
      margin-top: 130px;
      color: black;
      display: flex;
      justify-content: space-evenly;

      .offer-left {
        margin-right: 450px;
      }

      .offer-right {
        .offer-list {
          display: flex;
          justify-content: flex-start;
          align-items: center;
          margin-bottom: 20px;
          .offer-list-group {
            padding-left: 20px;

            p {
              font-size: 14px;
            }
          }
        }
      }
    }
  }
</style>