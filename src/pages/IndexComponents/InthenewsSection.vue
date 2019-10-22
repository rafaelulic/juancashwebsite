<template>
          <div class="in-the-news-section">
        <div class="container news-container">
          <div class="title">
            <h3>In the news</h3>
          </div>
          <div class="news-logo">
            <g-image src="~/assets/images/homepage/section-inthenews-cnn.jpg" />
            <g-image src="~/assets/images/homepage/section-inthenews-gma.jpg" />
            <g-image src="~/assets/images/homepage/section-inthenews-rappler.jpg" />
            <g-image src="~/assets/images/homepage/section-inthenews-coingeek.jpg" />
            <g-image src="~/assets/images/homepage/section-inthenews-yugatech.jpg" />
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
      height: 90px;
      border-radius: 50px;
      background-color: white;
      padding: 0 50px;
      display: flex;
      justify-content: space-around;
      align-items: center;
      width: 750px;
    }
  }
</style>