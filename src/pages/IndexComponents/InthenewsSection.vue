<template>
          <div class="in-the-news-section">
        <div class="container news-container">
          <div class="title">
            <h3>In the news</h3>
          </div>
          <div class="news-logo">
            <a href="https://www.rappler.com/technology/news/236310-juancash-juanexchange-launch-fintech-company-zybi-tech">
              <g-image src="~/assets/images/homepage/section-inthenews-rappler.jpg" />
            </a>
            <a href="http://bit.ly/JuanCashCNN">
              <g-image src="~/assets/images/homepage/section-inthenews-cnn.jpg" />
            </a>
            <a href="#">
              <g-image src="~/assets/images/homepage/section-inthenews-gma.jpg" />
            </a>
            <a href="https://coingeek.com/zybi-tech-launches-new-apps-to-aid-personal-finances-currency-trades/">
              <g-image src="~/assets/images/homepage/section-inthenews-coingeek.jpg" />
            </a>
            <a href="https://www.yugatech.com/news/juancash-juanexchange-financial-service-platforms-launched/#sthash.SZ1zoxME.dpbs%231dTLmoLb82LR6A87.97">
              <g-image src="~/assets/images/homepage/section-inthenews-yugatech.jpg" />
            </a>
          </div>
        </div>
      </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.in-the-news-section {
    background-color: $jcblue;
    height: 200px;

    .news-container {
      height: 200px;
      width: 800px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    h3 {
      margin-bottom: 20px;
    }

    .news-logo {
      min-height: 90px;
      border-radius: 50px;
      background-color: white;
      padding: 0 50px;
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      min-width: 800px;
    }
  }
</style>