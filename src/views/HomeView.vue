<template>
  <div class="home">
    <HomeHeader />

    <AboutView :isHomePage="isHomePage" />
    <ProductsShortPage />
    <HomeSkinCare />
    <!--
   
    <HomeCompanis />
    <HomeBlogandNews />
    <OurServices />
    <Footer /> -->
  </div>
</template>
<script>
import HomeHeader from "@/components/HomeHeader.vue";
import AboutView from "./AboutView.vue";
import ProductsShortPage from "@/components/ProductsShortPage.vue";
import HomeSkinCare from "@/components/HomeSkinCare.vue";
import HomeCompanis from "@/components/HomeCompanis.vue";
import HomeBlogandNews from "@/components/HomeBlogandNews.vue";
import OurServices from "@/components/OurServices.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "HomeView",
  data() {
    return {
      isHomePage: true,
    };
  },
  components: {
    HomeHeader,
    AboutView: AboutView,
    ProductsShortPage,
    HomeSkinCare,
    HomeCompanis,
    HomeBlogandNews,
    OurServices,
    Footer,
  },
};
</script>

<style >
*::-webkit-scrollbar {
  height: 6px;
  width: 6px;
}

*::-webkit-scrollbar-thumb {
  background-color: #205859;
  border-radius: 2.5px;
}
.about {
  background-color: #e5e3e4;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 967px;
  padding: 0 148px;
}
.about-images {
  border-radius: 50% 50% 0 0;
  background-size: contain;
}
.ab-img-left,
.ab-img-rigth {
  width: 410px;
  height: 550px;
}
.mb-3 {
  width: 566px;
  height: 62px;
}
@media (max-width: 1440px) {
  .about {
    max-width: 1440px;
    height: 630px;
    padding: 0 110px;
  }
  .about-info {
    width: 550px;
    height: 420px;
  }
  .beautyIsYouImg {
    max-width: 300px;
  }
  .ab-img-left,
  .ab-img-rigth {
    width: 310px;
    height: 450px;
  }
  .mb-3 {
    width: 500px;
  }
  .about-info-content {
    font-size: 17px;
  }
/* skin Care  */


}

@media (max-width: 1024px) {
  .about {
    max-width: 1024px;
    height: 500px;
    padding: 0 70px;
  }
  .ab-img-left,
  .ab-img-rigth {
    width: 210px;
    height: 200px;
  }
}
@media (max-width: 768px) {
  .about {
    max-width: 768px;
    height: 350px;
    padding: 0 40px;
  }
  .about-info {
    padding: 140px 0;
    width: 131px;
    height: 402px;
  }
  .beautyIsYouImg {
    max-width: 150px;
  }
  .about-info-content {
    font-size: 8px;
  }
  .mb-3 {
    width: 260px;
  }
  .ab-img-left,
  .ab-img-rigth {
    width: 162px;
    height: 200px;
  }
}
</style>
