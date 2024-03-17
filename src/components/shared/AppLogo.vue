<template>
  <div class="logo">
    <img src="../../assets/svg/Group.svg" alt="logo" class="logo__icon" />
    <p class="logo__text" :style="{ color: color }">RENTCARS</p>
  </div>
</template>

<script>
export default {
  name: "AppLogo",
  props: {
    color: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/variables";
.logo {
  display: flex;
  align-items: center;
  column-gap: 8px;

  &__text {
    font-family: "Poppins";
    font-size: "medium";
  }
}
</style>
