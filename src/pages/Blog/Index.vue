<template>
  <Layout>
    <div class="blog">
      <BlueBanner title="Blog" />
      <div class="container">
        <div class="blog-list">
          <div class="card-blog" :key="item.index" v-for="item of items">
            <div class="blog-banner">
              <g-image src="~/assets/images/merchant/photo-blog-5advantages.png"></g-image>
            </div>
            <div class="blog-title">
              <h3 class="text-blue">{{item.title}}</h3>
            </div>
            <div class="blog-excerpt">
              <p>{{item.excerpt}}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import BlueBanner from '~/components/BlueBanner.vue'
export default {
  components: { BlueBanner },
  data: function() {
    return {
      items: [
        {
          index: 0,
          title: "Blog 1",
          excerpt:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime eius quis laudantium quaerat dicta a placeat officiis qui, porro debitis, explicabo ratione magnam."
        },
        {
          index: 1,
          title: "Blog 2",
          excerpt:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime eius quis laudantium quaerat dicta a placeat officiis qui, porro debitis, explicabo ratione magnam."
        },
        {
          index: 1,
          title: "Blog 2",
          excerpt:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime eius quis laudantium quaerat dicta a placeat officiis qui, porro debitis, explicabo ratione magnam."
        },
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.blog {
  .container {
    .blog-list {
      width: 72%;
      margin: 0 auto;
      padding-top: 50px;
      display: flex;
      flex-flow: wrap;
      justify-content: flex-start;
      
      .card-blog {
        margin: 10px;   
        height: 350px;
        width: 460px;
        
      }
    }
  }
}
</style>
