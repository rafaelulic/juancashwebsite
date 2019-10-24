<template>
  <div class="banner">
    <h1>{{title}}</h1>
  </div>
</template>

<script>
export default {
    props: ['title']
}
</script>

<style lang="scss" scoped>
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
</style>