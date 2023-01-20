<template>
  <div class="about">
    <div class="about-images ab-img-left"></div>
    <div class="about-info">
      <p style="color: #469597" class="about-info-content mb-1">
        Alive every moment
      </p>
      <div>
        <img src="@/assets/images/about-quote.svg" class="beautyIsYouImg" />
      </div>
      <p class="about-info-content mb-3">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin lobortis
        sed sapien in pretium. Donec tincidunt, quam.
      </p>
      <img src="@/assets/images/about-signature.svg" v-if="!isHomePage" />
      <p class="about-info-content" v-if="!isHomePage">
        Founder & CEO of Chloro
      </p>
    </div>
    <div class="about-images ab-img-rigth"></div>
  </div>
</template>
<script>
export default {
  name: "AboutView",
  props: {
    isHomePage: {
      type: Boolean,
      default: false,
    },
  },
};
</script>
<style>
.about {
  min-width: 1920px;
  padding: 175px;
}
.about-info {
  padding: 85px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.ab-img-left {
  background-image: url(@/assets/images/about-img2.svg);
  background-repeat: no-repeat;
}
.ab-img-rigth {
  background-image: url(@/assets/images/about-img1.svg);
  background-repeat: no-repeat;
}
.about-info-content {
  font-size: 18px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 500;
  line-height: 170.02%;
  text-align: center;
  color: #05393a;
  margin-bottom: 8px;
}
.beautyIsYouImg {
  margin-bottom: 32px;
}
/* @media (max-width: 1500px) {

} */
/* @media (max-width: 1440px) {
}

@media (max-width: 1024px) {
}
@media (max-width: 768px) {
} */
</style>
