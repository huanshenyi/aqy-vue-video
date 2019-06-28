<template>
  <div>
    <home-header></home-header>
    <home-nav></home-nav>
    <home-search></home-search>
    <home-swiper></home-swiper>
    <home-tubiao></home-tubiao>
    <home-list></home-list>
    <home-infomation></home-infomation>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeNav from './components/Nav'
import HomeSearch from './components/Search'
import HomeSwiper from './components/Swiper'
import HomeTubiao from './components/Tubiao'
import HomeList from './components/List'
import HomeInfomation from './components/Infomation'

export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeNav,
    HomeSearch,
    HomeSwiper,
    HomeTubiao,
    HomeList,
    HomeInfomation
  }
}
</script>

<style scoped>

</style>
