<template>
  <div class="hero">
    <div class="hero__container">
      <AppHeader />
      <div class="hero__content">
        <h1 class="hero__content-title">
          Find, book and rent a car
          <span class="hero__content-span">Easily</span>
        </h1>
        <h3 class="hero__content-text">
          Get a car wherever and whenever you need it with your IOS and Android
          device.
        </h3>
        <ul class="hero__content-links">
          <li>
            <a href="https://play.google.com/"
              ><img
                class="hero__content-img"
                src="../../assets/img/google.jpg"
                alt="google play"
            /></a>
          </li>
          <li>
            <a href="https://www.apple.com/"
              ><img
                class="hero__content-img"
                src="../../assets/img/app-store.jpg"
                alt="app store"
            /></a>
          </li>
        </ul>
      </div>
      <div class="hero__search">
        <ul class="hero__search-list">
          <li class="hero__search-item">
            <img
              class="hero__search-image"
              src="../../assets/svg/location.svg"
              alt="location icon"
            />
            <div class="hero__search-content">
              <h4 class="hero__search-title">Location</h4>
              <p class="hero__search-text">Search your location</p>
            </div>
          </li>
          <li class="hero__search-item">
            <img
              class="hero__search-image"
              src="../../assets/svg/calendar.svg"
              alt="calendar icon"
            />
            <div class="hero__search-content">
              <h4 class="hero__search-title">Pickup date</h4>
              <p class="hero__search-text"></p>
            </div>
          </li>
          <li class="hero__search-item">
            <img
              class="hero__search-image"
              src="../../assets/svg/calendar.svg"
              alt="calendar icon"
            />
            <div class="hero__search-content">
              <h4 class="hero__search-title">Return date</h4>
              <p class="hero__search-text"></p>
            </div>
          </li>
          <li>
            <button class="hero__search-btn" type="button">Search</button>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import AppHeader from "../Header/AppHeader.vue";
export default {
  name: "AppHero",
  components: {
    AppHeader,
  },
};
</script>

<style lang="scss" scoped>
.hero {
  background-image: url("../../assets/img/car.png"),
    url("../../assets/img/hero-bg.png");
  background-repeat: no-repeat;
  background-position-x: right;
  background-position-y: 150px, 0;

  &__container {
    padding: 48px 160px;
  }

  &__content {
    display: flex;
    flex-direction: column;
    row-gap: 40px;
    width: 390px;
    height: 239px;
    margin-top: 157px;

    &-title {
      color: #242424;
      font-family: "Poppins";
      font-weight: "Semi-bold";
      font-size: 48px;
    }

    &-span {
      padding-bottom: 10px;
      color: #1572d3;
      background-image: url("../../assets/img/vector.png");
      background-repeat: no-repeat;
      background-position-y: 53px;
    }

    &-text {
      color: #272727;
      font-family: "Poppins";
      font-weight: "Regular";
      font-size: 18px;
    }

    &-links {
      display: flex;
      column-gap: 12px;
    }
  }

  &__search {
    width: 1120px;
    padding: 18px 32px;
    margin: 150px auto 0 auto;

    &-list {
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 4px 16px 12px -2px rgba(158, 198, 255, 0.29);
    }

    &-item {
      padding: 5px;
      display: flex;
      column-gap: 20px;
    }

    &-content {
      border-right: 2px solid rgb(130, 129, 129);
      padding-right: 50px;
    }

    &-title {
      font-family: "Poppins";
      font-weight: "Regular";
      font-size: 20px;
      color: #242424;
    }

    &-text {
      margin-top: 4px;
      font-family: "Poppins";
      font-weight: "Bold";
      font-size: 14px;
      color: #242424;
    }

    &-btn {
      background: transparent;
      border: none;
      font-family: "Poppins";
      font-weight: "Regular";
      font-size: 22px;
      color: #1572d3;
      cursor: pointer;
    }
  }
}
</style>
