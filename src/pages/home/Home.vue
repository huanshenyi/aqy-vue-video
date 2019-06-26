<template>
  <div>
    <home-header></home-header>
    <home-nav></home-nav>
    <home-search></home-search>
    <home-swiper></home-swiper>
    <home-tubiao></home-tubiao>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeNav from './components/Nav'
import HomeSearch from './components/Search'
import HomeSwiper from './components/Swiper'
import HomeTubiao from './components/Tubiao'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeNav,
    HomeSearch,
    HomeSwiper,
    HomeTubiao
  }
}
</script>

<style scoped>

</style>
