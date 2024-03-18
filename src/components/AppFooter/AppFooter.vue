<template>
  <footer class="footer">
    <div class="footer__main">
      <div class="footer__main-contacts">
        <AppLogo :color="logoColor" />
        <div class="footer__main-location">
          <div class="footer__main-item">
            <img src="../../assets/svg/location.svg" alt="location" />
            <p class="footer__main-text">
              25566 Hc 1, Glenallen, Alaska, 99588, USA
            </p>
          </div>
          <div class="footer__main-item">
            <img src="../../assets/svg/call.svg" alt="phone" />
            <p class="footer__main-text">+603 4784 273 12</p>
          </div>
          <div class="footer__main-item">
            <img src="../../assets/svg/sms.svg" alt="message" />
            <p class="footer__main-text">rentcars@gmail.com</p>
          </div>
        </div>
      </div>
      <div class="footer__main-product">
        <h3 class="footer__main-title">Our Product</h3>
        <div class="footer__main-content">
          <p class="footer__main-text">Career</p>
          <p class="footer__main-text">Car</p>
          <p class="footer__main-text">Packages</p>
          <p class="footer__main-text">Features</p>
          <p class="footer__main-text">Priceline</p>
        </div>
      </div>
      <div class="footer__main-resources">
        <h3 class="footer__main-title">Resources</h3>
        <div class="footer__main-content">
          <p class="footer__main-text">Download</p>
          <p class="footer__main-text">Help Centre</p>
          <p class="footer__main-text">Guides</p>
          <p class="footer__main-text">Partner Network</p>
          <p class="footer__main-text">Cruises</p>
          <p class="footer__main-text">Developer</p>
        </div>
      </div>
      <div class="footer__main-about">
        <h3 class="footer__main-title">About Rentcars</h3>
        <div class="footer__main-content">
          <p class="footer__main-text">Why choose us</p>
          <p class="footer__main-text">Our Story</p>
          <p class="footer__main-text">Investor Relations</p>
          <p class="footer__main-text">Press Center</p>
          <p class="footer__main-text">Advertise</p>
        </div>
      </div>
      <div class="footer__main-follow">
        <h3 class="footer__main-title">Follow Us</h3>
        <div class="footer__main-links">
          <a href="https://www.facebook.com/"
            ><img src="../../assets/svg/facebook.svg" alt="facebook"
          /></a>
          <a href="https://www.instagram.com/"
            ><img src="../../assets/svg/instagram.svg" alt="instagram"
          /></a>
          <a href="https://www.youtube.com/"
            ><img src="../../assets/svg/youtube.svg" alt="youtube"
          /></a>
        </div>
      </div>
    </div>
    <p class="footer__copyright">
      Copyright 2023 ・ Rentcars, All Rights Reserved
    </p>
  </footer>
</template>

<script>
import AppLogo from "../shared/AppLogo.vue";
export default {
  name: "AppFooter",
  components: {
    AppLogo,
  },
  data() {
    return {
      logoColor: "#FFFFFF",
    };
  },
};
</script>

<style lang="scss" scoped>
.footer {
  padding: 40px 160px;
  background: #051c34;

  &__main {
    display: flex;
    padding-bottom: 64px;
    border-bottom: 2px solid #575757;

    &-contacts {
      width: 191px;
    }

    &-location {
      margin-top: 32px;
      display: flex;
      flex-direction: column;
      row-gap: 24px;
    }

    &-item {
      display: flex;
      align-items: center;
      column-gap: 8px;
    }

    &-text {
      color: #d6d6d6;
      font-family: "Poppins";
      font-weight: 400;
      font-size: 14px;
    }

    &-title {
      color: #ffffff;
      font-family: "Poppins";
      font-weight: 500;
      font-size: 16px;
    }

    &-product {
      margin-left: 193px;
      width: 96px;
    }

    &-resources {
      margin-left: 96px;
      width: 111px;
    }

    &-about {
      margin-left: 81px;
      width: 125px;
    }

    &-follow {
      margin-left: 67px;
      width: 104px;
    }

    &-content {
      margin-top: 32px;
      display: flex;
      flex-direction: column;
      row-gap: 16px;
    }

    &-links {
      margin-top: 32px;
      display: flex;
      column-gap: 16px;
    }
  }

  &__copyright {
    margin-top: 32px;
    color: #d6d6d6;
    font-family: "Poppins";
    font-weight: 400;
    font-size: 12px;
  }
}
</style>
