<template>
  <header :class="[isHome ? 'header' : 'header-2']">
    <nav class="navbar container">
      <div class="logo">
        <g-link to="/">
          <g-image alt="JuanCash Logo" :src="require('~/assets/images/homepage/logo-juancash'+[isHome ? '' : blue]+'.png')" />
        </g-link>
      </div>

      <div class="nav-link-container">
        <ul class="nav-link-wrapper">
          <li>
            <g-link to="/">Home</g-link>
          </li>
          <li>
            <g-link to="/business">Business</g-link>
          </li>
          <li>
            <g-link to="/merchants">Merchants</g-link>
          </li>
          <li class="learn-more">
            LEARN MORE <font-awesome-icon icon="caret-down" />
            <ul class="dropdown">
              <li>
                <g-link to="/blog">Blog</g-link>
              </li>
              <li>
                <g-link to="/promos">Promos</g-link>
              </li>
            </ul>
          </li>
          <li>
            <g-link to="/contact">Contact Us</g-link>
          </li>
          <li>
            <a href="https://www.facebook.com/JuanCashOfficial/">
              <g-image alt="JuanCash Facebook" :src="require('~/assets/images/homepage/social-facebook'+[isHome ? '' : blue]+'.png')" />
            </a>
          </li>
          <li>
            <a href="">
              <g-image alt="JuanCash WeChat" :src="require('~/assets/images/homepage/social-wechat'+ [isHome ? '' : blue] +'.png')" />
            </a>
          </li>
          <li>
            <a href="https://twitter.com/juancash__">
              <g-image alt="JuanCash Twittter" :src="require('~/assets/images/homepage/social-twitter'+ [isHome ? '' : blue] +'.png')" />
            </a>
          </li>
          <li>
            <a href="https://www.instagram.com/juancashofficial/">
              <g-image alt="JuanCash Instagram" :src="require('~/assets/images/homepage/social-instagram'+ [isHome ? '' : blue] +'.png')" />
            </a>
          </li>
          <li>
            <button class="button">English &nbsp; <font-awesome-icon icon="caret-down" /></button>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isHome: false,
      blue: "-blue",
    }
  },
  beforeMount () {
    let currentRoute = this.$route.path

    if (currentRoute === '/'){
      this.isHome = true
    } else {
      this.isHome = false
    }
  }

}
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  background: $jcblue;
  height: 80px;
  
  .navbar {
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: flex-start;

    .nav-link-container {
      flex: 1;
      .nav-link-wrapper {
        list-style: none;
        height: 80px;
        margin: 0;

        display: flex;
        justify-content: flex-end;
        align-items: center;

        li {
          padding-left: 20px;
          color: white;

          a {
            text-decoration: none;
            color: white;
            text-transform: uppercase;
          }
        }

        li.learn-more {
          cursor: pointer;

          &:hover {
            .dropdown {
              display: block;
            }
          }

          .dropdown {
            background: white;
            position: absolute;
            display: none;
            list-style-type: none;
            width: 108px;

            li {
              padding: 10px;
              a {
                color: black;
              }

              &:hover {
                background: $jcgold;
              }
            }
          }
        }
      }
    }
  }
}

.header-2 {
  width: 100%;
  background: white;
  height: 80px;
  
  .navbar {
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: flex-start;

    .nav-link-container {
      flex: 1;
      .nav-link-wrapper {
        list-style: none;
        height: 80px;
        margin: 0;

        display: flex;
        justify-content: flex-end;
        align-items: center;

        li {
          padding-left: 20px;
          color: black;

          a {
            text-decoration: none;
            color: black;
            text-transform: uppercase;
          }
        }

        li.learn-more {
          cursor: pointer;

          &:hover {
            .dropdown {
              display: block;
            }
          }

          .dropdown {
            background: $jcblue;
            position: absolute;
            display: none;
            list-style-type: none;
            width: 112px;

            li {
              padding: 10px;
              a {
                color: white;
              }

              &:hover {
                background: $jcgold;
              }
            }
          }
        }
      }
    }
  }
}
</style>

