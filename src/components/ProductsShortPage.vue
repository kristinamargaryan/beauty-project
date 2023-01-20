<template>
  <div class="products">
    <div class="products-about">
      <h2 class="products-title">Our Product</h2>
      <p class="products-about-text">
        Lorem ipsum dolor sit amet, consec tetur adipiscing elit.
      </p>
      <button class="shop-now-btn">
        <span class="shop-now-btn-name">
          SHOP NOW
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
    <div class="carousel">
      <VueperSlides :isSlides="isSlides" />
    </div>
  </div>
</template>

<script>
import VueperSlides from "@/components/VueperSlides.vue";
export default {
  name: "ProductsShortPage",
  components: {
    VueperSlides,
  },
  data: () => ({
    isSlides: [
      {
        src: require("../assets/images/product1.png"),
        title: "A photographer shows the beauty transition",
      },
      {
        src: require("../assets/images/product2.png"),
        title: "Natural look: The evolution of implants",
      },
      {
        src: require("../assets/images/product3.png"),
        title: "Russian prosecutor seeks to Dolce and Gabbana",
      },
      {
        src: require("../assets/images/product4.png"),
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

<style >
.products {
  min-width: 1920px;
  background-color: #5ba199;
  height: 720px;
  padding: 10px 0 10px 148px;
  display: flex;
  align-items: center;
}
.products-about {
  text-align: left;

  padding-right: 98px;
}
.carousel {
  height: 720px;
  width: 1550px;
  padding-top: 112px;
}
.products-title {
  width: 379px;
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 400;
  font-size: 76px;
  line-height: 126.52%;
  color: #ffffff;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
.products-about-text {
  font-family: "Montserrat";
  width: 370px;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 170.02%;
  color: #ffffff;
  margin-bottom: 42px;
}
.shop-now-btn {
  width: 226px;
  height: 66px;
  border-radius: 60px;
  border: none;
}
.shop-now-btn-name {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 170.02%;
  text-align: right;
  color: #469597;
}
.vueperslide,
.vueperslide__image {
  background-position: 50%;
  width: 359px;
  height: 359px;
  border-radius: 250px 250px 0px 0px;
}
.vueperslides__parallax-wrapper {
  height: 359px;
}

@media (max-width: 1440px) {
  .products {
    max-width: 1440px;
  }
}
@media (max-width: 1024px) {
  .products {
    max-width: 1024px;
    height: 530px;
    padding: 10px 0 10px 70px;
  }
  .products-title {
    font-size: 50px;
  }
  .shop-now-btn {
    width: 170px;
    height: 50px;
  }
  .products-about {
    padding-right: 15px;
  }
  .carousel {
    padding-top: 24px;
    height: 332px;
    width: 694px;
  }
  .vueperslide,
  .vueperslide__image {
    background-position: 50%;
    width: 259px;
    height: 259px;
  }
}
@media (max-width: 768px) {
  .products {
    max-width: 768px;
    height: 351px;
    padding: 10px 0 10px 40px;
  }
  .products-about-text {
    font-size: 8px;
    margin: 0;
    width: 170px;
    padding-bottom: 20px;
  }
  .products-title {
    width: 269px;
  }
  .shop-now-btn {
    width: 120px;
    height: 30px;
  }
  .shop-now-btn-name {
    font-size: 11px;
  }
  .vueperslide,
  .vueperslide__image {
    background-position: 50%;
    width: 200px;
    height: 200px;
  }
  .vueperslides__parallax-wrapper {
    height: 200px;
  }
}

.vueperslides__bullet--active .default {
  border-width: 0;
}
.vueperslides__bullet .default {
  width: 0;
  height: 0;
}
/* @media (max-width: 1500px) {

}  


@media (max-width: 1024px) {
}
 */
</style>
