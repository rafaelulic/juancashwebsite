<template>
  <div class="wrapper">
    <div class="accordion" @click="toggleItem">
      <span class="title">
        <g-image src="~/assets/images/merchant/ico-faq-listing.png"></g-image>
        <span><slot name="title"></slot></span>
      </span>
    </div>
    <div v-show="show" class="content">
      <slot name="content"></slot>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data: function() {
    return {
      show: false
    };
  },
  methods: {
    toggleItem: function() {
      this.show = !this.show;
    }
  }
};
</script>
<style lang='scss' scoped>
.wrapper {
  margin: 0 auto;
  width: 90%;
  padding: 10px;
}
.accordion {
  display: flex;
  cursor: pointer;

  margin: 0;
}
.title {
  margin: 0;
  color: $jcblue;
  span {
    font-size: 18px;
    font-weight: 600;
    // line-height: 1.56;
  }
  img {
      margin-right: 10px;
      vertical-align: middle;
  }
}

.content {
  text-align: left;
  width: 100%;
  padding: 20px;
  font-size: 14px;
  font-weight: 600;
}
</style>