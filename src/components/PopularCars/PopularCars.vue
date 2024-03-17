<template>
  <section class="popular-section">
    <h2 class="popular-section__name">POPULAR RENTAL DEALS</h2>
    <h3 class="popular-section__title">Most popular cars rental deals</h3>
    <ul class="popular-section__list">
      <CarCard v-for="car in cars" :key="car.id" :car="car" />
    </ul>
    <button class="popular-section__button">
      Show all vehicles<span class="popular-section__span"
        ><img src="../../assets/svg/arrow-right.svg" alt="arrow right"
      /></span>
    </button>
  </section>
</template>

<script>
import CarCard from "./CarCard.vue";
import carsList from "./carsList";
export default {
  name: "PopularCars",
  components: {
    CarCard,
  },
  data() {
    return {
      cars: [...carsList],
    };
  },
};
</script>

<style lang="scss" scoped>
.popular-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 84px 160px;

  &__name {
    color: #1572d3;
    width: 226px;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 14px;
    background: #c5ddf6;
    padding: 16px 32px;
    border-radius: 8px;
  }

  &__title {
    margin-top: 32px;
    color: #333333;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 38px;
  }

  &__list {
    display: flex;
    column-gap: 32px;
    margin-top: 64px;
  }

  &__button {
    display: flex;
    justify-content: center;
    column-gap: 8px;
    color: #4e4e4e;
    margin-top: 64px;
    padding: 14px 34px;
    background: transparent;
    border: 2px solid #959595;
    border-radius: 8px;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 14px;
    cursor: pointer;
  }
}
</style>
