<template>
  <div class="home">
    <home-header></home-header>
    <home-nav></home-nav>
    <home-search></home-search>
    <home-swiper></home-swiper>
    <home-tubiao></home-tubiao>
    <home-list></home-list>
    <home-infomation></home-infomation>
    <home-footer></home-footer>
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
import HomeFooter from './components/Footer'
import axios from 'axios'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeNav,
    HomeSearch,
    HomeSwiper,
    HomeTubiao,
    HomeList,
    HomeInfomation,
    HomeFooter
  },
  mounted () {
    this.getDjangoData()
  },
  methods: {
    getDjangoData: function () {
      axios.get('http://127.0.0.1:8000/goods/').then((response) => {
        console.log(response.data)
      })
    }
  }
}
</script>

<style scoped lang="stylus">
.home
  background #ffffff
</style>
