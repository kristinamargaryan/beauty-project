<template>
  <div class="about">
  <div>
    <img class="about-img img-left" src="@/assets/images/about-img1.svg" :class="{'img-height' : isHomePage }" alt="img">
  </div>
  <div class="about-info">
    <p style="color:#469597" class="about-info-content mb-1"> Alive every moment </p>
    <img src="@/assets/images/about-quote.svg" class="beautyIsYouImg" />
    <p class="about-info-content mb-3"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin lobortis sed sapien in pretium. Donec tincidunt, quam. </p>
    <img src="@/assets/images/about-signature.svg"  v-if="!isHomePage"/>
    <p class="about-info-content" v-if="!isHomePage"> Founder & CEO of Chloro </p>
  </div>
  <div>
    <img class="about-img img-rigth" src="@/assets/images/about-img2.svg" :class="{'img-height' : isHomePage }" alt="img"/>
  </div>
  </div>
</template>
<script>
export default{
name: 'AboutView',
props:{
  isHomePage:{
    type: Boolean,
    default: false
  }
}
}
</script>
<style>
.about{
  background-color: #E5E3E4;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 967px;
  padding: 0 148px;
}
.about-info {
  padding: 85px;
}
.about-img {
  width: 455px;
  height: 666px;
}
.about-info-content {
  font-size: 20px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  line-height: 170.02%;
  text-align: center;
  color: #DDBEAA;
  margin-bottom: 8px;
}
.beautyIsYouImg{
  margin-bottom: 32px;
}
.img-height{
  height: 469px;
}
</style>