<template>
  <Layout>
    <div class="faq">
      <BlueBanner title="Frequently Asked Questions" />
      <div class="container">
        <div class="accordion-wrapper">
          <div class="question">
            <div class="answer"></div>
          </div>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import BlueBanner from "~/components/BlueBanner.vue";

export default {
  components: { BlueBanner },
  metaInfo: {
    title: "FAQs"
  },
  data() {
    return {
      myItems: [
        {
          title: "What is JuanCash?",
          value: "JuanCash is a mobile application that holds electronic and virtual currencies, and performs financial transactions.",
          category: "JuanCash Basics"
        },
        {
          title: "How do I register for a JuanCash account?",
          value: "You may download the JuanCash app via PlayStore and AppStore. You will be needing a mobile number and an active email address for the registration.",
          category: "JuanCash Basics"
        },
        {
          title: "What animal smells like popcorn?",
          value: "Binturongs smell like popcorn.",
          category: "JuanCash Basics"
        }
      ]
    }
  }
}
</script>

<style lang='scss'>
  .container {
    height: 100vh;

    .faq-wrapper {
      
    }
  }
</style>