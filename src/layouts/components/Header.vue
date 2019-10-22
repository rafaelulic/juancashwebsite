<template>
  <header class="header">
    <nav class="navbar container">
      <div class="logo">
        <g-link to="/">
          <g-image alt="JuanCash Logo" src="~/assets/images/homepage/logo-juancash.png" />
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
            LEARN MORE
            <ul class="dropdown">
              <li>
                <g-link>Blog</g-link>
              </li>
              <li>
                <g-link>News</g-link>
              </li>
            </ul>
          </li>
          <li>
            <g-link>Contact Us</g-link>
          </li>
          <li>
            <g-link>
              <g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-facebook.png" />
            </g-link>
          </li>
          <li>
            <g-link>
              <g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-wechat.png" />
            </g-link>
          </li>
          <li>
            <g-link>
              <g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-twitter.png" />
            </g-link>
          </li>
          <li>
            <g-link>
              <g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-instagram.png" />
            </g-link>
          </li>
          <li>
            <button class="button">English</button>
            <!-- <g-link><g-image alt="JuanCash Facebook" src="~/assets/images/homepage/social-facebook.png" /></g-link> -->
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {};
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
          padding-left: 10px;
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
</style>