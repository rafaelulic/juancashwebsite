<template>
  <Layout>
    <div class="faq">
      <BlueBanner title="Frequently Asked Questions" />
      <div class="container">
        <Accordion />
      </div>
    </div>
  </Layout>
</template>

<script>
import BlueBanner from "~/components/BlueBanner.vue"
import Accordion from './components/Accordion.vue'


export default {
  components: { BlueBanner, Accordion },
  metaInfo: {
    title: "FAQs"
  },
  methods: {
    activate() {
      this.isActive = !this.isActive
      this.isVisible = !this.isVisible
    }
  }
}
</script>

<style lang='scss' scoped>
  .container {
    min-height: 100vh;
    margin-top: 20px;
  }
</style>