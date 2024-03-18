<template>
  <Carousel class="carousel" :items-to-show="2" :wrap-around="true">
    <Slide v-for="item in items" :key="item.id">
      <Card class="carousel__item" :item="item" />
    </Slide>

    <template #addons>
      <Navigation />
    </template>
  </Carousel>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Navigation, Slide } from "vue3-carousel";
import Card from "./Card.vue";
import people from "./people.js";
import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "WrapAround",
  components: {
    Carousel,
    Slide,
    Navigation,
    Card,
  },
  data() {
    return {
      items: [...people],
    };
  },
});
</script>

<style lang="scss" scoped>
.carousel {
  width: 100%;
  height: 586px;
  margin-top: 80px;
}

.carousel__item {
  height: 586px;
  width: 794px;
  background-color: #ffffff;
  border-radius: 24px;
  display: flex;

  align-items: center;
}

.carousel__prev,
.carousel__next {
}

.carousel__slide {
}

.carousel__track {
  transform-style: preserve-3d;
}

.carousel__slide--sliding {
  transition: 0.5s;
}

.carousel__slide {
  height: 438px;
  opacity: 0.9;
  transform: rotateY(-20deg);
}

.carousel__slide--next {
}

.carousel__slide--prev {
}

.carousel__slide--active {
  height: 586px;
  opacity: 1;
}
</style>
