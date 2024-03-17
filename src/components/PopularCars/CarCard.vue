<template>
  <li class="car-card">
    <div class="car-card__image-container">
      <img class="car-card__image" :src="car.image" :alt="car.name" />
    </div>
    <div class="car-card__descr">
      <h4 class="car-card__name">{{ car.name }}</h4>
      <div class="car-card__popular">
        <img src="../../assets/svg/star.svg" alt="star" />
        <p class="car-card__popular-rating">{{ car.rating }}</p>
        <p class="car-card__popular-reviews">({{ car.reviews }} reviews)</p>
      </div>
      <ul class="car-card__char">
        <li class="car-card__char-container">
          <img src="../../assets/svg/user.svg" alt="user" />
          <p class="car-card__char-text">{{ car.passagers }} Passagers</p>
        </li>
        <li class="car-card__char-container">
          <img src="../../assets/svg/transmission.svg" alt="transmission" />
          <p class="car-card__char-text">{{ car.transmission }}</p>
        </li>
        <li class="car-card__char-container">
          <img src="../../assets/svg/snow.svg" alt="snow" />
          <p class="car-card__char-text">{{ car.condition }}</p>
        </li>
        <li class="car-card__char-container">
          <img src="../../assets/svg/door.svg" alt="door" />
          <p class="car-card__char-text">{{ car.doors }} Doors</p>
        </li>
      </ul>
      <div class="car-card__price">
        <p class="car-card__price-name">Price</p>
        <p class="car-card__price-number">
          ${{ car.price }} <span class="car-card__price-span">/ day</span>
        </p>
      </div>
      <button class="car-card__button" type="button">
        Rent Now
        <span
          ><img
            src="../../assets/svg/arrow-right-white.svg"
            alt="arrow right white"
        /></span>
      </button>
    </div>
  </li>
</template>

<script>
export default {
  name: "CarCard",
  props: {
    car: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.car-card {
  width: 256px;
  height: 405px;
  border-radius: 16px;
  box-shadow: -1px 14px 17px -6px rgb(169, 169, 200);

  &__image-container {
    width: 256px;
    height: 155px;
    padding: 38px 24px 32px 24px;
  }

  &__image {
    width: 208px;
    height: 85px;
  }

  &__descr {
    padding: 0 24px;
  }

  &__name {
    color: #262626;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 16px;
  }

  &__popular {
    display: flex;
    align-items: center;
    column-gap: 6px;
    margin-top: 12px;
  }

  &__popular-rating {
    color: #000000;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 12px;
  }

  &__popular-reviews {
    color: #808080;
    font-family: "Poppins";
    font-weight: 400;
    font-size: 12px;
  }

  &__char {
    margin-top: 16px;
    padding-bottom: 24px;
    border-bottom: 2px solid #e0e0e0;
    display: grid;
    justify-content: space-between;
    row-gap: 8px;

    grid-template-columns: auto auto;

    &-container {
      display: flex;
      align-items: center;
      column-gap: 4px;
    }

    &-text {
      color: #959595;
      font-family: "Poppins";
      font-weight: 400;
      font-size: 12px;
    }
  }

  &__price {
    display: flex;
    margin-top: 24px;
    justify-content: space-between;

    &-name {
      color: #595959;
      font-family: "Poppins";
      font-weight: 400;
      font-size: 14px;
    }

    &-number {
      color: #292929;
      font-family: "Poppins";
      font-weight: 600;
      font-size: 16px;
    }

    &-span {
      color: #9c9c9c;
      font-family: "Poppins";
      font-weight: 400;
      font-size: 14px;
    }
  }

  &__button {
    width: 100%;
    margin-top: 24px;
    display: flex;
    justify-content: center;
    column-gap: 8px;
    padding: 10px 57px;
    background: #1572d3;
    color: #ffffff;
    font-family: "Poppins";
    font-weight: 500;
    font-size: 14px;
    border-radius: 14px;
    border: none;
    cursor: pointer;
  }
}
</style>
