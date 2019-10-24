<template>
  <Layout>
    <div class="contact">
      <BlueBanner title="Contact Us" />
      <div class="blue-bg">

      </div>
      <div class="container">
        <div class="contact-left">
          adf
        </div>
        <div class="contact-right">
          <g-image src="~/assets/images/contact/section-img-inner-contact.png"></g-image>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import BlueBanner from "~/components/BlueBanner.vue"
export default {
  components: { BlueBanner },
  metaInfo: {
    title: "Contact Us"
  }
}
</script>

<style lang='scss'>
.contact {
  background-position: center;
  
  .blue-bg {
    background: url("~@/assets/images/contact/bg-inner-contact.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 400px;
  }

  .container {
    margin-top: -380px;
    display: grid;
    grid-template-columns: repeat(2, 1fr); 
  }
}
</style>