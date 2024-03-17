<template>
  <AppContainer>
    <Hero />
    <main>
      <ChooseUs />
      <PopularCars />
      <AboutUs />
    </main>
  </AppContainer>
</template>

<script>
import AppContainer from "./components/shared/AppContainer.vue";
import Hero from "./components/Hero/Hero.vue";
import ChooseUs from "./components/ChooseUs/ChooseUs.vue";
import PopularCars from "./components/PopularCars/PopularCars.vue";
import AboutUs from "./components/About/AboutUs.vue";

export default {
  name: "App",
  components: {
    AppContainer,
    Hero,
    ChooseUs,
    PopularCars,
    AboutUs,
  },
};
</script>

<style lang="scss" scoped>
#app {
  min-height: 100vh;
  font-family: Poppins, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.content {
}
</style>
