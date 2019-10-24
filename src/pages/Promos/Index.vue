<template>
  <Layout>
    <div class="promo">
      <BlueBanner title="Promos" />
      <div class="container">
        <div class="promo-list">
          <div class="card-promo" :key="item.index" v-for="item of items">
            <div class="promo-banner">
              <g-image src="~/assets/images/merchant/photo-promo-prelaunch-promo.png"></g-image>
            </div>
            <div class="promo-title">
              <h3 class="text-blue">{{item.title}}</h3>
            </div>
            <div class="promo-excerpt">
              <p>{{item.excerpt}}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import BlueBanner from "~/components/BlueBanner.vue";
export default {
  components: { BlueBanner },
  data: function() {
    return {
      items: [
        {
          index: 0,
          title: "Promo 1",
          excerpt:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime eius quis laudantium quaerat dicta a placeat officiis qui, porro debitis, explicabo ratione magnam."
        },
        {
          index: 1,
          title: "Promo 2",
          excerpt:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime eius quis laudantium quaerat dicta a placeat officiis qui, porro debitis, explicabo ratione magnam."
        },
        {
          index: 1,
          title: "Promo 2",
          excerpt:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime eius quis laudantium quaerat dicta a placeat officiis qui, porro debitis, explicabo ratione magnam."
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.promo {
  .banner {
    background: $jcblue;
    height: 160px;
    display: flex;
    justify-content: center;
    align-items: flex-end;

    h1 {
      color: white;
    }
  }
  .container {
    .promo-list {
      width: 72%;
      margin: 0 auto;
      padding-top: 50px;
      display: flex;
      flex-flow: wrap;
      justify-content: flex-start;

      .card-promo {
        margin: 10px;
        height: 350px;
        width: 460px;
      }
    }
  }
}
</style>
