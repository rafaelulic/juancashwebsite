<template>
  <div class="business-solution-section">
    <div class="container">
      <div class="business-solutions-wrapper">
        <div class="row">
          <div class="left">
            <g-image src="~/assets/images/business/section-img-inner-business-innovating.png"></g-image>
          </div>
          <div class="right">
            <h2>Innovating Business Solutions Through Convenient And Secure Payments</h2>
            <p>JuanCash offers the latest scan-to-pay mobile payment solutions suited to your business requirements.</p>
						<br>
            <p>Our seamless payment solutions allow your business to accept payments using the latest QR technology that is convenient &amp; secured.</p>
						<br>
            <p>JuanCash merchants enjoy full-access and benefits to after-sales transactions with our back-end solutions for posting and reporting.</p>
          </div>
        </div>
        <div class="row">
          <div class="left">
            <h1>Be a JuanCash Merchant</h1>
            <button class="btn-large">
              Join Now
              <g-image src="~/assets/images/homepage/button-ico-more.png" />
            </button>
            <div class="business-merchant-img">
							<g-image src="~/assets/images/business/section-img-inner-business-merchant.jpg" />
						</div>						
          </div>
          <div class="right">
            <h3>Sign up as a JuanCash merchant and enjoy the following benefits:</h3>
						<div class="card-wrapper">
							<div class="card" :key="item.index" v-for="item in items">
								<g-image :src="require('~/assets/images/business/'+item.image)"/>
								<p>{{item.text}}</p>
							</div>
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
          image: "section-img-merchant-benefits-1.png",
          text: "Backend Payment Settlement"
        },
        {
          index: 1,
          image: "section-img-merchant-benefits-2.png",
          text: "Provide real-time posting and transaction"
        },
        {
          index: 2,
          image: "section-img-merchant-benefits-3.png",
          text: "Offer secured payment solution"
        },
        {
          index: 3,
          image: "section-img-merchant-benefits-4.png",
          text: "Provide share infrastructure and network"
        },
        {
          index: 4,
          image: "section-img-merchant-benefits-5.png",
          text: "Lower rates than most credit card"
        },
        {
          index: 5,
          image: "section-img-merchant-benefits-6.png",
          text: "Inclusion in our Advertising and Promotional Activities"
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

.business-solution-section {
  background-image: url("~@/assets/images/business/bg-inner-business.png");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 790px;
	margin-top: -80px;

	.container {
		padding: 0 100px;
	}
	
	p {color:white;}

  h1 {
    font-size: 44px;
    width: 390px;
		color: white;
		padding-top: 110px;
  }
	.business-merchant-img {
		margin-top: 90px;
	}

  .card {
		width: 168px;
		height: 250px;
		border-radius: 8px;
		border: solid 2px $jcgold;
		background-color: white;
		margin-bottom: 20px;

		display: flex;
		flex-flow: column;
		justify-content: center;
		align-items: center;
		
		p {
			font-size: 14px;
			font-weight: 600;
			text-align: center;
			color: #09426d;
			width: 150px;
		}
	}
	
	.card-wrapper {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;

		margin-top: 50px;	

	}

  .business-solutions-wrapper {
    padding-top: 30px;

    h2 {
      color: white;
    }

    .row {
      display: grid;
      grid-template-columns: repeat(2, 1fr);

      .right {
        margin-left: 50px;
        width: 600px;
      }
    }
  }
}
</style>