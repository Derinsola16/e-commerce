<template>
  <main class="slider container">
    <carousel
      :nav="false"
      :margin="15"
      :stagePadding="1"
      :loop="true"
      :items="4"
      :autoplay="true"
      :dots="true"
    >
      <img src="@/assets/image29.png" class="" />

      <img src="@/assets/image6.png" />

      <img src="@/assets/image5.png" />

      <img src="@/assets/image7.png" />

      <img src="@/assets/image29.png" class="" />

      <img src="@/assets/image1.png" />

      <img src="@/assets/image5.png" />

      <img src="@/assets/image7.png" />

      <img src="@/assets/image29.png" class="" />

      <img src="@/assets/image6.png" />

      <img src="@/assets/image5.png" />

      <img src="@/assets/image7.png" />

      <img src="@/assets/image29.png" class="" />

      <img src="@/assets/image9.png" />

      <img src="@/assets/image5.png" />

      <img src="@/assets/image7.png" />
    </carousel>
  </main>
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  components: { carousel }
};
</script>

<style lang="scss" scoped>
.slider {
  img {
    width: 200px;
    height: 200px;
    object-fit: scale-down;
    // background: red !important;
  }

  // .owl-dot.active {
  //   background-color: #ffb300 !important;
  // }

  // .owl-dots.owl-dot span {
  //   width: 6px !important;
  //   height: 6px !important;
  //   margin: 5px 3px !important;
  //   background: red !important;
  //   display: block !important;
  //   // -webkit-backface-visibility: visible;
  //   transition: opacity 200ms ease !important;
  //   border-radius: 30px !important;
  // }

  // .owl-theme .owl-dots .owl-dot.active span,
  // .owl-theme .owl-dots .owl-dot:hover span {
  //   background: blue;
  // }
  // .owl-theme .owl-dots .owl-dot span {
  //   background: #ffb300 !important;
  // }
}
</style>
