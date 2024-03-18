<template>
  <section class="download-app">
    <div class="download-app__content">
      <h2 class="download-app__name">DOWNLOAD</h2>
      <h3 class="download-app__title">
        Download Rentcars App for<span class="download-app__span"> FREE</span>
      </h3>
      <p class="download-app__text">
        For faster, easier booking and exclusive deals.
      </p>
      <div class="download-app__links">
        <a href="https://play.google.com/"
          ><img src="../../assets/img/google.jpg" alt="google play"
        /></a>
        <a href="https://www.apple.com"
          ><img src="../../assets/img/app-store.jpg" alt="app store"
        /></a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "DownloadApp",
};
</script>

<style lang="scss" scoped>
.download-app {
  background: #ffffff;
  padding: 72px 81px 100px 160px;
  background-image: url("../../assets/img/vector-a.png"),
    url("../../assets/img/iPhone.png");
  background-repeat: no-repeat;
  background-position-x: 0, calc(100% - 81px);
  background-position-y: -100px, 72px;

  &__content {
    width: 460px;
  }

  &__name {
    color: #1572d3;
    width: 146px;
    font-weight: 500;
    font-size: 14px;
    background: #c5ddf6;
    padding: 16px 32px;
    border-radius: 8px;
  }

  &__title {
    margin-top: 24px;
    color: #282828;
    font-weight: 500;
    font-size: 38px;
  }

  &__span {
    color: #1572d3;
  }

  &__text {
    margin-top: 40px;
    color: #3e3e3e;
    font-weight: 400;
    font-size: 16;
  }

  &__links {
    display: flex;
    margin-top: 40px;
    column-gap: 16px;
  }
}
</style>
