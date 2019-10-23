<template>
  <Layout>
    <div class="business">

      <BannerSection />
      <BusinessSolutionSection />
      <BusinessAgencySection />
    </div>
  </Layout>
</template>

<script>
import BannerSection from './components/BannerSection.vue'
import BusinessSolutionSection from './components/BusinessSolutionSection.vue'
import BusinessAgencySection from './components/BusinessAgencySection.vue'

export default {
  metaInfo: {
    title: 'Business'
  },
  components: {
    BannerSection,
    BusinessSolutionSection,
    BusinessAgencySection,
  }
}
</script>

<style lang='scss'>

</style>