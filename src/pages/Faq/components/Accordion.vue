<template>
  <div class="accordion-wrapper">
    <button class="level-1-accordion" @click="activateLvl1()">JuanCashBasics <font-awesome-icon icon="caret-down" :style="{transform: isActive ? 'rotate(180deg)' : ''}" /></button>
    <div class="level-1-panel" :style="{display: isActive ? 'block' : 'none'}">
      <div v-for="basic in basics" :key="basic.title">
        <BaseAccordion>
          <template v-slot:title>{{ basic.title }}</template>

          <template v-slot:content>
            <div>{{ basic.text }}</div>
          </template>
        </BaseAccordion>
      </div>
    </div>
    <button class="level-1-accordion" @click="activateLvl2()">Services <font-awesome-icon icon="caret-down" :style="{transform: isActive2 ? 'rotate(180deg)' : ''}"/></button>
    <div class="level-1-panel" :style="{display: isActive2 ? 'block' : 'none'}">
      <div v-for="service in services" :key="service.title">
        <BaseAccordion>
          <template v-slot:title>{{ service.title }}</template>

          <template v-slot:content>
            <div>{{ service.text }}</div>
          </template>
        </BaseAccordion>
      </div>
    </div>
    <button class="level-1-accordion" @click="activateLvl3()">Other Concerns <font-awesome-icon icon="caret-down" :style="{transform: isActive3 ? 'rotate(180deg)' : ''}"/></button>
    <div class="level-1-panel" :style="{display: isActive3 ? 'block' : 'none'}">
      <div v-for="other in others" :key="other.title">
        <BaseAccordion>
          <template v-slot:title>{{ other.title }}</template>

          <template v-slot:content>
            <div>{{ other.text }}</div>
          </template>
        </BaseAccordion>
      </div>
    </div>
  </div>
</template>

<script>
import BaseAccordion from "./BaseAccordion";
export default {
  components: {
    BaseAccordion
  },
    data () {
        return {
           isActive: false,
           isActive2: false,
           isActive3: false,
           basics: [
            {
              title: "What is JuanCash",
              text: "JuanCash is a mobile application that holds electronic and virtual currencies, and performs financial transactions."
            },
            {
              title: "How do I Register for a JuanCash account",
              text: "You may download the JuanCash app via PlayStore and AppStore. You will be needing a mobile number and an active email address for the registration"
            },
            {
              title: "How many accounts can I activate?",
              text: "Your personal mobile number serves as your account. With this, you can only activate one (1) JuanCash wallet per mobile number."
            }, 
            {
              title: "What is JuanCash QR and how can I use it?",
              text: "JuanCash QR is a unique code that can be used for purchasing and payment when scanned via JuanCash app."
            },
            {
              title: "Where and how can I check my balance?",
              text: "JuanCash QR is a unique code that can be used for purchasing and payment when scanned via JuanCash app."
            },
            {
              title: "Where and how can I check my balance?",
              text: "You can check your wallet’s balance at the top portion of the app’s main dashboard."
            }
          ],
          services: [
            {
              title: "What services can I avail with JuanCash?",
              text: "JuanCash offers a variety of services you can utilize such as bills payment, mobile loading, sending and receiving money, making purchases and virtual currency trading."
            },
            {
              title: "How do I use JuanCash for payments?",
              text: "You can see all the services and transactions you can utilize in JuanCash’s main dashboard. Simply select the icon of your preferred service."
            },
            {
              title: "Which merchants are included in JuanCash’s payment transactions?",
              text: "Please refer to the merchant's page."
            },
            {
              title: "Why do I need to upgrade my tier? Is there a fee when I want to upgrade my account?",
              text: "You need to upgrade your tier in order to avail and upgrade features such as addition in the minimum and maximum cash-in and cash-out amount, fund transfer, bills payment and virtual currency trading. NO, there is no fee when upgrading your account."
            },
            {
              title: "I cannot upgrade my tier. What can I do?", 
              text: "You can check the following tips 1. Make sure you have a stable internet connection. 2. If you can’t upload a file, make sure that the files are clear and of the following file types: JPEG/JPG, 3.PNG PDF, DOC or EXCEL files will not be accepted."
            }
          ],
          others: [
            {
              title: "What should I do if I lost my phone which bears my JuanCash account? Can I still access the account with another mobile number?",
              text: "You can still access your account via your new mobile number. Simply log-in using your registered mobile number and password. To prevent others from accessing your account from a stolen device, change and your new mobile number and register it to your account."
            },
            {
              title: "I can’t access or open my JuanCash account.",
              text: "You may contact JuanCash at support@juancash.com for other concerns regarding logging in to your account."
            },
            {
              title: "List of valid IDs I need to upgrade my tier",
              text: ""
            }
          ]
        }
    },
    methods: {
        activateLvl1 () {
            this.isActive = !this.isActive
        },  
        activateLvl2 () {
            this.isActive2 = !this.isActive2
        },
        activateLvl3 () {
            this.isActive3 = !this.isActive3
        }
    }
}
</script>

<style lang="scss" scoped>
.accordion-wrapper {
  width: 80%;
  margin: 20px auto;

  .level-1-accordion {
    background: white;
    border: 2px solid $jcblue;
    border-radius: 8px;
    color: $jcblue;
    cursor: pointer;
    font-size: 22px;
    font-weight: 600;
    text-align: left;
    padding: 20px;
    margin-bottom: 10px;
    width: 100%;
    
    &:focus {
        outline: none;
    }

    svg {
      float: right;
      color: $jcgold;
    }
  }
}
</style>