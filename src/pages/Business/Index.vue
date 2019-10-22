<template>
  <Layout>
    <BannerSection />
    <BusinessSolutionSection />
  </Layout>
</template>

<script>
import BannerSection from './components/BannerSection.vue'
import BusinessSolutionSection from './components/BusinessSolutionSection.vue'

export default {
  metaInfo: {
    title: 'Business'
  },
  components: {
    BannerSection,
    BusinessSolutionSection,
  }
}
</script>

<style lang='scss'>

</style>