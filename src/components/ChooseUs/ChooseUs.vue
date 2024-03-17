<template>
  <section class="choose-section">
    <div class="choose-section__content">
      <h2 class="choose-section__name">WHY CHOOSE US</h2>
      <h3 class="choose-section__title">
        We offer the best experience with our rental deals
      </h3>
      <ul class="choose-section__list">
        <li class="choose-section__item">
          <img
            class="choose-section__icon"
            src="../../assets/svg/wallet.svg"
            alt="wallet"
          />
          <div class="choose-section__item-content">
            <h4 class="choose-section__item-title">Best price guaranteed</h4>
            <p class="choose-section__item-text">
              Find a lower price? We’ll refund you 100% of the difference.
            </p>
          </div>
        </li>
        <li class="choose-section__item">
          <img
            class="choose-section__icon"
            src="../../assets/svg/user-tick.svg"
            alt="user"
          />
          <div class="choose-section__item-content">
            <h4 class="choose-section__item-title">Experience driver</h4>
            <p class="choose-section__item-text">
              Don’t have driver? Don’t worry, we have many experienced driver
              for you.
            </p>
          </div>
        </li>
        <li class="choose-section__item">
          <img
            class="choose-section__icon"
            src="../../assets/svg/24-support.svg"
            alt="24 support"
          />
          <div class="choose-section__item-content">
            <h4 class="choose-section__item-title">24 hour car delivery</h4>
            <p class="choose-section__item-text">
              Book your car anytime and we will deliver it directly to you.
            </p>
          </div>
        </li>
        <li class="choose-section__item">
          <img
            class="choose-section__icon"
            src="../../assets/svg/messages-2.svg"
            alt="messages"
          />
          <div class="choose-section__item-content">
            <h4 class="choose-section__item-title">24/7 technical support</h4>
            <p class="choose-section__item-text">
              Have a question? Contact Rentcars support any time when you have
              problem.
            </p>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "ChooseUs",
};
</script>

<style lang="scss" scoped>
.choose-section {
  display: flex;
  justify-content: flex-end;
  margin-top: 92px;
  padding-right: 130px;
  padding-bottom: 91px;
  background-image: url("../../assets/img/audi.png"),
    url("../../assets/img/vector-a.png");
  background-repeat: no-repeat;
  background-position-y: 150px, 0;

  &__content {
    width: 576px;
    height: 617px;
  }

  &__name {
    color: #1572d3;
    width: 181px;
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
    margin-top: 56px;
    width: 455px;
    display: flex;
    flex-direction: column;
    row-gap: 40px;
  }

  &__item {
    display: flex;
    align-items: center;
    column-gap: 24px;

    &-title {
      color: #000000;
      font-family: "Poppins";
      font-weight: 500;
      font-size: 20px;
    }

    &-text {
      margin-top: 20px;
      color: #6d6d6d;
      font-family: "Poppins";
      font-weight: normal;
      font-size: 16px;
    }
  }

  &__icon {
    padding: 20px;
    border-radius: 16px;
    background: #c5ddf6;
  }
}
</style>
