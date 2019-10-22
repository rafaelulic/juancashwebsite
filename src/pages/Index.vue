<template>
  <Layout>
    <div id="index">
      <BannerSection />
      <SkipLinesSection />
      <VirtualCurrenciesSection />
      <BusinessSection />
      <SafeSection />
      <CashlessSection />
      <InthenewsSection />
    </div>
  </Layout>
</template>

<script>
import SafeSection from './IndexComponents/SafeSection'
import BannerSection from './IndexComponents/BannerSection'
import SkipLinesSection from './IndexComponents/SkipLinesSection'
import VirtualCurrenciesSection from './IndexComponents/VirtualCurrencies'
import BusinessSection from './IndexComponents/BusinessSection'
import CashlessSection from './IndexComponents/CashlessSection'
import InthenewsSection from './IndexComponents/InthenewsSection'

export default {
  metaInfo: {
    title: "Your All-in-Juan Financial App"
  },
  components: {
    BannerSection,
    SkipLinesSection,
    VirtualCurrenciesSection,
    BusinessSection,
    SafeSection,
    CashlessSection,
    InthenewsSection    
  }
}
</script>

<style lang='scss' scoped>
#index {
  color: white;

}
</style>
