<template>
  <section class="about-section">
    <h2 class="about-section__name">TESTIMONIALS</h2>
    <h3 class="about-section__title">What peole say about us?</h3>
    <Carousel />
  </section>
</template>

<script>
import Carousel from "./Carousel.vue";
export default {
  name: "AboutUs",
  components: {
    Carousel,
  },
};
</script>

<style lang="scss" scoped>
.about-section {
  display: flex;
  flex-direction: column;

  align-items: center;
  padding: 53px 0;

  background: #ecf5ff;
  background-image: url("../../assets/img/about-left.png"),
    url("../../assets/img/about-right.png");
  background-repeat: no-repeat;
  background-position-x: 137px, calc(100% - 106px);
  background-position-y: 90px, 0;

  &__name {
    color: #1572d3;
    width: 161 px;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 14px;
    background: #c5ddf6;
    padding: 16px 32px;
    border-radius: 8px;
  }

  &__title {
    margin-top: 24px;
    color: #333333;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 38px;
  }
}
</style>
