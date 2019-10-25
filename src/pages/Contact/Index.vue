<template>
  <Layout>
    <div class="contact">
      <BlueBanner title="Contact Us" />
      <div class="blue-bg"></div>
      <div class="container">
        <div class="contact-left">
          <form action>
            <label for>Name:</label>
            <input type="text" name id />
            <label for>Email Address:</label>
            <input type="text" name id />
            <label for>Phone:</label>
            <input type="text" name id />
            <label for>Company:</label>
            <input type="text" name id />
            <label for>Message:</label>
            <textarea name id cols="30" rows="10"></textarea>
            <button class="btn-large">Submit</button>
          </form>
        </div>
        <div class="contact-right">
          <g-image src="~/assets/images/contact/section-img-inner-contact.png"></g-image>
          <p>8th Floor IMET BPO Tower, <br>Metropolitan Avenue Roxas Boulevard, <br>Pasay City, Philippines</p>
          <p>(02) 8878-0889
            <br>apps@zybitech.com
            <br>info@zybitech.com</p>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import BlueBanner from "~/components/BlueBanner.vue";

export default {
  components: { BlueBanner},
  metaInfo: {
    title: "Contact Us"
  }
};
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

  form {
    display: block;
    width: 100%;

    %form-elements {
      display: block;
      padding: 12px 20px;
      margin: 15px 0;
      box-sizing: border-box;
      width: 100%;
      outline: none;
      border: 1px solid $jclightblue;
      font-size: 18px;
    }

    %form-focus {
      border: 3px solid $jclightblue;
    }

    label {
      display: block;
      width: 100%;
      margin: 8px 0;
      font-size: 14px;
      font-weight: 600;
    }

    input[type] {
      @extend %form-elements;
      height: 48px;
      
      &:focus {
        @extend %form-focus;  
      }
    }

    textarea {
      @extend %form-elements;

      &:focus {
        @extend %form-focus;  
      }
    }
  }

  .container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    margin-top: -380px;
    margin-bottom: 100px;

    .contact-left {
      max-width: 500px;
    }

    .contact-right {
      p {
        margin-top: 50px;
        padding-left: 70px;
      }
    }

  }
}
</style>