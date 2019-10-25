<template>
  <div class="merchants-section">
    <div class="search-section">
      <div class="left">
        <p>Enter merchant name below to find merchants near you</p>
        <form action>
          <input type="text" placeholder="Enter merchant name"/>
          <button>Search</button>
        </form>
      </div>
      <div class="right">
        <p>Search for a merchant in your city</p>
        <form action>
          <select name id>
            <option value>Select a city</option>
            <option value></option>
          </select>
        </form>
      </div>
    </div>

    <div class="result-section">
      <div class="container">
        <div class="merchant-card" :key="item.index" v-for="item of items">
          <div class="left">
            <div class="mechant-name">
              <h3>{{item.name}}</h3>
            </div>
            <div class="merchant-address">
              <span>{{item.address}}</span>
            </div>
            <div class="merchant-contact">
              <g-image src="~/assets/images/merchant/merchants-ico-phone.png"></g-image>
              <span>{{item.phone}}</span>
            </div>
          </div>
          <div class="right">
            <g-image src="~/assets/images/merchant/ico-merchant-map.png"></g-image>
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
          name: "Ministop 1",
          address:
            "Bank of Commerce Aduana Bldg. No. 409-a Soriano St. Intramuros, Manila",
          phone: "0918 5621732"
        },
        {
          index: 1,
          name: "Ministop 2",
          address:
            "Bank of Commerce Aduana Bldg. No. 409-a Soriano St. Intramuros, Manila",
          phone: "0918 5621732"
        },
        {
          index: 2,
          name: "Ministop 3",
          address:
            "Bank of Commerce Aduana Bldg. No. 409-a Soriano St. Intramuros, Manila",
          phone: "0918 5621732"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.merchants-section {
  p {
    color: white;
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 20px;
  }
  form {
    display: flex;
    width: 100%;

    input[type="text"] {
      flex: 75%;
      width: 100%;
      padding: 12px 20px;
      box-sizing: border-box;
      font-size: 14px;
    }

    button {
      flex: 25%;
      border: none;
      background-color: $jcgold;
      color: white;
      height: 44px;
      font-size: 18px;
      font-weight: 600;
      text-transform: uppercase;
      width: 100%;
    }

    select {
      width: 55%;
      height: 44px;
      padding-left: 10px;
    }

    ::placeholder {
        color:#b2b2b2;
    }
  }

  .search-section {
    display: flex;
    height: 160px;
    .left {
      display: flex;
      flex-flow: column;
      justify-content: center;
      align-items: flex-start;
      background-color: $jcblue;
      padding-left: 17%;
      padding-right: 2.5%;
      width: 100%;
    }

    .right {
      display: flex;
      flex-flow: column;
      justify-content: center;
      align-items: flex-start;
      padding-left: 2.5%;
      padding-right: 17%;
      width: 100%;
      background-color: #4dcff8;
      border-left: 1px solid white;
    }
  }

  .result-section {
    .container {
      padding: 40px;
      display: flex;
      flex-flow: wrap;

      .merchant-card {
        margin: 20px;
        width: 480px;
        height: 160px;
        border: solid 2px $jclightblue;
        padding: 20px;
        display: flex;
        align-items: center;

        h3 {
          color: $jcblue;
          margin-bottom: 10px;
        }

        .merchant-address {
          margin-bottom: 10px;
          font-size: 14px;
          font-weight: bold;
        }

        .merchant-contact {
            display: flex;
            justify-content: flex-start;
            align-items: center;

            img {
                margin-right: 10px;
            }
        }

        .right {
            padding-left: 50px;
        }
      }
    }
  }
}
</style>