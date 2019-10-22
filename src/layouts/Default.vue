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
<style lang="scss">
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.layout {
  font-family: 'Open Sans', sans-serif;

  display: flex;
  flex-flow: column;
  
  footer {
    flex-grow: 1;
  }
}

</style>