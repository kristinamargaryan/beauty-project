<template>
  <div class="blog-and-news">
    <div class="blogandnews-content">
      <div>
        <img
          class="blogandnews-content-title"
          src="@/assets/images/BlogAndNewsIcon.svg"
          alt=""
        />
      </div>
      <div>
        <p class="blogandnews-content-info">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin
          lobortis sed sapien in pretium. Donec tincidunt, quam.
        </p>
      </div>
    </div>
    <div class="blogandnews-containers">
      <div
        class="all-containers first-container"
        v-for="(item, i) in items"
        :key="i"
      >
        <img
          class="first-container-img all-container-img"
          :src="item.src"
          alt=""
        />
        <div class="all-container-info-box">
          <div class="min-box">
            <p class="all-container-info">{{ item.title }}</p>
            <button class="container-button">
              <span>
                READ MORE
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
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
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
    ],
  }),
};
</script>

<style>
.blog-and-news {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 1070px;
  background: #e5e3e4;
  padding: 125px 215px;
}
.blogandnews-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-bottom: 80px;
}
.blogandnews-content-title {
  padding-bottom: 20px;
  width: 554px;
  height: 96px;
}
.blogandnews-content-info {
  width: 682px;
  height: 62px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 170.02%;
  text-align: center;
  color: #205859;
}
.blogandnews-containers {
  display: flex;
}
.all-containers {
  width: 471px;
  height: 547px;
  margin-right: 40px;
}
.all-containers .all-container-info-box {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  width: 471px;
  height: 212px;
  background: #469597;
  padding: 35px 35px;
}
.all-container-img {
  height: 335px;
  border-radius: 550px 550px 0px 0px;
}

.all-container-info {
  width: 403.5px;
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 126.52%;
  color: #ffffff;
  text-align: justify;
}
.container-button {
  height: 27px;
  border: none;
  border-bottom: 1px solid #5ba199;
  background: #469597;
  color: #e5e3e4;
}
.min-box {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
</style>
