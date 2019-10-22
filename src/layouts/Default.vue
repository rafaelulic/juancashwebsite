<template>
  <div class="layout">
    <Header/>
    <slot />
    <Footer/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
export default {
  components: {
    Header,
    Footer
  }
}

</script>
<style lang="scss" scoped>
.layout {font-family: 'Open Sans', sans-serif;}

</style>