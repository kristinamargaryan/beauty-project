<template>
  <div class="home-header">
    <div class="home-header-left-side">
      <p class="quote">
        A whole <span class="motserrat-style"><i>new world</i></span> , a whole
        <span class="motserrat-style"><i>new look</i></span>
      </p>
      <p class="quote-text">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin lobortis
        sed sapien in pretium. Donec tincidunt, quam vestibulum.
      </p>
      <button class="more-info">
        <span class="more-info-btn">
          DISCOVER MORE
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="16"
            height="16"
            fill="currentColor"
            class="bi bi-arrow-right"
            viewBox="0 0 16 16"
          >
            <path
              fill-rule="evenodd"
              d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"
            />
          </svg>
        </span>
      </button>
    </div>
    <div class="home-header-carousel">
      <VueperSlides :isSlides="isSlides" />
    </div>
  </div>
</template>

<script>
import VueperSlides from "@/components/VueperSlides.vue";
export default {
  name: "HomeHeader",
  components: {
    VueperSlides,
  },
  data: () => ({
    isSlides: [
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "A photographer shows the beauty transition",
      },
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "Natural look: The evolution of implants",
      },
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "Russian prosecutor seeks to Dolce and Gabbana",
      },
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "Natural look: The evolution of implants",
      },
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "Russian prosecutor seeks to Dolce and Gabbana",
      },
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "Natural look: The evolution of implants",
      },
      {
        src: require("../assets/images/blogandnewsphoto.svg"),
        title: "Russian prosecutor seeks to Dolce and Gabbana",
      },
    ],
  }),
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Cormorant:wght@300&family=Montserrat:wght@100&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:wght@300&family=Montserrat:wght@100&display=swap");
.home-header {
  display: flex;
  justify-content: space-between;
  height: 1005px;
  min-width: 1920px;
  background: #469597;
  padding: 140px 0 130px 200px;
}
.home-header-left-side {
  margin-top: 35px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  max-width: 667px;
  padding-right: 185px;
}
.quote {
  width: 667px;
  height: 290px;
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 400;
  font-size: 95px;
  line-height: 106px;
  color: #ffffff;
  text-align: left;
}
.quote-text {
  width: 566px;
  height: 93px;
  text-align: left;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 170.02%;
  color: #ffffff;
  margin-top: 58px;
}
.more-info {
  width: 270px !important;
  min-height: 66px !important;
  background: #ffffff;
  border-radius: 60px;
  border: none;
  margin-top: 76px;
}
.more-info-btn {
  width: 270px;
  height: 66px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 170.02%;
  color: #469597;
}
.motserrat-style {
  font-family: "Montserrat";
}
.home-header-carousel {
  height: 670px;
  width: 1000px;
}

@media (max-width: 1440px) {
  .home-header {
    max-width: 1440px;
    height: 625px;
    padding-left: 12px;
    justify-content: flex-start;

  }
  .home-header-left-side {
    max-width: 600px;
    margin-top: 1px;
    padding: 100px;
  }
  .quote {
    font-size: 40px;
    width: 292px;
    height: 195px;
    line-height: 50px;
    margin-bottom: 0;
  }
  .quote-text {
    margin: 0;
    width: 370px;
    font-size: 12px;
  }
  .home-header-carousel {
    height: 450px;
    width: 600px;
  }
  .more-info {
    margin-top: 0px;
    width: 175px !important;
    min-height: 40px !important;
  }
  .more-info-btn {
    font-size: 11px;
  }
}
@media (max-width: 1200px) {
  .home-header {
    max-width: 1200px;
    padding-left: 150px;
  }
  .home-header-carousel {
    height: auto;
  }
  .vueperslides__parallax-wrapper {
    height: 360px;
  }
}
@media (max-width: 1024px) {
  .home-header {
    max-width: 1024px;
    max-height: 600px;
    padding-left: 70px;
  }
  .quote {
    font-size: 35px;
    width: 280px;
  }
  .quote-text {
    width: 350px;
    font-size: 11px;
  }
  .more-info {
    margin-top: 15px;
    width: 160px !important;
  }
  .home-header-carousel {
    height: 500px;
    width: 750px;
  }
  .home-header-left-side {
    margin-top: 15px;
    max-width: 450px;
  }
  .vueperslide,
  .vueperslide__image {
    width: 200px !important;
    height: 318px;
  }
  .vueperslides__parallax-wrapper {
    height: 318px;
  }
}
@media (max-width: 768px) {
  .home-header {
    max-width: 768px;
    max-height: 400px;
    padding-left: 47px;
    padding-top: 100px;
  }

  .quote {
    font-size: 25px;
    width: 160px;
    line-height: 30px;
  }
  .quote-text {
    width: 250px;
    font-size: 8px;
    padding-right: 10px;
  }
  .more-info {
    width: 100px !important;
    min-height: 30px !important;
  }

  .more-info-btn {
    font-size: 8px;
    height: 0px;
    display: flex;
    flex-direction: row;
    align-items: center;
  }
  .home-header-carousel {
    height: auto;
  }
  .vueperslide,
  .vueperslide__image {
    width: 130px !important;
    height: 200px;
  }
  .vueperslides__parallax-wrapper {
    height: 250px;
  }
  .vueperslides__parallax-wrapper {
    height: 50;
  }
}

@media (max-width: 320px) {
  .home-header {
    width: 320px;
    height: 240px;
    flex-direction: column;
    align-items: center;
  }
}
</style>
