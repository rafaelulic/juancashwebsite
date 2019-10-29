<template>
  <Layout>
    <div class="faq">
      <BlueBanner title="Frequently Asked Questions" />
      <div class="container">
        <div class="accordion-wrapper">
          <div class="tab">
            <button @click="activate()" :class="{active: isActive}">JuanCash Basics</button>            
            <button>Services</button>            
            <button>Other Concerns</button>            
          </div>
          <div class="tab-content">
            JuanCash Basics
          </div>
          <div class="tab-content">
            Services
          </div>
          <div class="tab-content">
            Other Services
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
  methods: {
    activate() {
      this.isActive = !this.isActive
    }
  }, 
  data() {
    return {
      isActive: false,
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

    .tab {
      width: 100%;
      background-color: white;
      margin-top: 20px;
      border-bottom: 2px solid $jcblue;

      .active {
        background-color: $jcblue;
      }

      button {
        border: none;
        background-color: #f2f2f2;
        height: 40px;
        border-radius: 15px 15px 0 0;
        padding: 40px;
        min-width: 30%;
        font-size: 18px;
        margin-right: 5px;
        cursor: pointer;
        &:focus {
          outline: none;
        }
      }
    }
  }
</style>