<template>
  <div class="business-agency-section">
    <div class="container">
      <div class="row">
        <div class="left">
          <h2>Apply to the JuanPay Agency System</h2>
          <p>JuanPay Agency System is a financial brand integrated in JuanCash mobile application that offers financial services to micro businesses.</p>
          <br />
          <p>JuanPay Agency System will cater to those who want to start a business by offering financial services in their area. With the use of JuanCash App they will be able to transact bills payment, mobile load, gaming, remittance etc.</p>
          <button class="btn-large">
            Join Now
            <g-image src="~/assets/images/homepage/button-ico-more.png" />
          </button>
        </div>
        <div class="right">
          <g-image src="~/assets/images/business/section-img-inner-business-agency.png"></g-image>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.business-agency-section {
  margin-top: 342px;
  height: 440px;
  background-color: $jcblue;
  color: white;

  .container {
    padding: 0 100px;
    h2 {
      color: white;
    }

    .row {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-template-rows: 440px;
      justify-items: start;
      align-items: center;
    }

    p {
      width: 600px;
    }

    .btn-large {
      margin-top: 20px;
    }
  }
}
</style>