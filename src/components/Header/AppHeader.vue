<template>
  <header class="header">
    <AppLogo :color="logoColor" />
    <nav class="heder__nav">
      <ul class="header__nav-list">
        <li class="header__nav-item">
          <a class="header__nav-link">Become a renter</a>
        </li>
        <li class="header__nav-item">
          <a class="header__nav-link">Rental deals</a>
        </li>
        <li class="header__nav-item">
          <a class="header__nav-link">How it work</a>
        </li>
        <li class="header__nav-item">
          <a class="header__nav-link">Why choose us</a>
        </li>
      </ul>
    </nav>
    <ul class="header__auth">
      <li>
        <button class="header__auth-button" type="button">Sign In</button>
      </li>
      <li>
        <button class="header__auth-button" type="button">Sign Out</button>
      </li>
    </ul>
  </header>
</template>

<script>
import AppLogo from "../shared/AppLogo.vue";
export default {
  name: "AppHeader",
  components: { AppLogo },
  data() {
    return {
      logoColor: "#1572D3",
    };
  },
};
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;

  &__nav {
    &-list {
      display: flex;
      column-gap: 40px;
    }

    &-item {
      color: #484848;
      font-family: "Poppins";
      font-weight: medium;
      font-size: 16px;
    }
  }

  &__auth {
    display: flex;
  }

  &__auth-button {
    color: #484848;
    background: transparent;
    border: none;
    font-family: "Poppins";
    font-weight: medium;
    font-size: 16px;
    cursor: pointer;
  }
}
</style>
