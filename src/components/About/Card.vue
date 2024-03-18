<template>
  <div class="card">
    <img class="card__image" :src="item.src" :alt="item.name" />
    <div class="card__context">
      <p class="card__context-stars">
        <span class="card__context-span">{{ item.stars.toFixed(1) }}</span>
        stars
      </p>
      <div class="card__stars-container">
        <img src="../../assets/svg/star.svg" alt="star" />
        <img src="../../assets/svg/star.svg" alt="star" />
        <img src="../../assets/svg/star.svg" alt="star" />
        <img src="../../assets/svg/star.svg" alt="star" />
        <img src="../../assets/svg/star.svg" alt="star" />
      </div>
      <p class="card__text">{{ item.text }}</p>
      <p class="card__name">{{ item.name }}</p>
      <p class="card__from">{{ item.from }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "PeopleCard",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.card {
  &__image {
    border-radius: 20px;
  }

  &__context {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 40px;

    &-span {
      color: #383838;
      font-weight: 500;
      font-size: 64px;
    }

    &-stars {
      color: #383838;
      font-weight: 500;
      font-size: 24px;
    }
  }

  &__stars-container {
    margin-top: 24px;
    display: flex;
    column-gap: 4px;
  }

  &__text {
    text-align: left;
    margin-top: 196px;
    color: #282828;
    font-weight: 400;
    font-size: 18px;
  }

  &__name {
    margin-top: 80px;
    color: #252525;
    font-weight: 500;
    font-size: 24px;
  }

  &__from {
    margin-top: 16px;
    color: #838383;
    font-weight: 400;
    font-size: 14px;
  }
}
</style>
