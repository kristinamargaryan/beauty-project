<template>
  <vueper-slides
    :arrows="false"
    :infinite="false"
    class="no-shadow"
    :dragging-distance="200"
    :breakpoints="{ 800: { visibleSlides: 2, slideMultiple: 2 } }"
    :gap="3"
    :slide-ratio="1 / 4"
    slide-multiple
    :visible-slides="3"
  >
    <vueper-slide
      class="vueper-img"
      v-for="slide in isSlides"
      :key="slide"
      :image="slide.src"
    />

    <!-- <svg
      xmlns="http://www.w3.org/2000/svg"
      width="16"
      height="16"
      fill="currentColor"
      class="bi bi-arrow-left-short"
      viewBox="0 0 16 16"
    >
      <path
        fill-rule="evenodd"
        d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"
      />
    </svg> -->
  </vueper-slides>
</template>
<script>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
export default {
  components: { VueperSlides, VueperSlide },
  props: {
    isSlides: {
      type: Object,
      default: false,
    },
  },
};
</script>


