<template>
  <div class="home"></div>
</template>

<template>
  <splide @splide:mounted="onMounted" @splide:arrows:mounted="onArrowsMounted">
    <splide-slide>
      <img
        src="https://i.guim.co.uk/img/media/c9b0aad22638133aa06cd68347bed2390b555e63/0_477_2945_1767/master/2945.jpg?width=1200&height=1200&quality=85&auto=format&fit=crop&s=97bf92d90f51da7067d00f8156512925"
      />
    </splide-slide>
    <splide-slide>
      <img
        src="https://images.unsplash.com/photo-1520315342629-6ea920342047?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=1000&q=80"
      />
    </splide-slide>
    <splide-slide>
      <img
        src="https://i.guim.co.uk/img/media/7a633730f5f90db3c12f6efc954a2d5b475c3d4a/0_138_5544_3327/master/5544.jpg?width=1200&height=1200&quality=85&auto=format&fit=crop&s=27c09d27ccbd139fd0f7d1cef8f7d41d"
      />
    </splide-slide>
  </splide>
</template>
<style>
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}
</style>

<script>
import { Splide, SplideSlide } from "@splidejs/vue-splide";
import "@splidejs/splide/dist/css/themes/splide-default.min.css";
export default {
  data() {
    return {
      options: {
        rewind: true,
        width: 800,
        perPage: 1,
        gap: "1rem",
      },
      name: "Home",
      components: {
        Splide,
        SplideSlide,
      },
      // methods: {
      //   onMounted(splide) {
      //     // do something
      //   },

      //   onArrowsMounted(splide, prev, next) {
      //     // do something
      // },
      // },
    };
  },
};
</script>
