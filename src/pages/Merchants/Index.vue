<template>
  <Layout>
    <BannerSection />
    <MerchantsSection />
  </Layout>
</template>

<script>
import BannerSection from './components/BannerSection.vue'
import MerchantsSection from './components/MerchantsSection.vue'
export default {
  metaInfo: {
    title: 'Merchants'
  },
  components: {
    BannerSection,
    MerchantsSection
  }
}
</script>

<style lang='scss'>

</style>
