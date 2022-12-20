<template>
  <div class="home">
    <HomeHeader/>
    <AboutView
    :isHomePage="isHomePage"/>
    <ProductsShortPage/>
    <HomeSkinCare />
  </div>
</template>
<script>
import HomeHeader from '@/components/HomeHeader.vue'
import AboutView from './AboutView.vue'
import ProductsShortPage from '@/components/ProductsShortPage.vue'
import HomeSkinCare from '@/components/HomeSkinCare.vue'
export default {
  name: 'HomeView',
  data(){
    return {
      isHomePage: true
    }
  },
  components: {
    HomeHeader,
    AboutView: AboutView,
    ProductsShortPage,
    HomeSkinCare
  }
}
</script>
