<template>
  <div>
    <home-header></home-header>
    <home-nav></home-nav>
    <home-search></home-search>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeNav from './components/Nav'
import HomeSearch from './components/Search'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeNav,
    HomeSearch
  }
}
</script>

<style scoped>

</style>
