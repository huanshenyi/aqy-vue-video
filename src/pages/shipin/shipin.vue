<template>
 <div class="home">
   <home-header></home-header>
   <fa-slo></fa-slo>
   <title-bar></title-bar>
   <home-footer></home-footer>
 </div>
</template>

<script>
import HomeHeader from '../home/components/Header'
import FaSlo from './components/faslo'
import TitleBar from './components/Titlebar'
import HomeFooter from '../home/components/Footer'
export default {
  name: 'shipin',
  components: {
    HomeHeader,
    FaSlo,
    HomeFooter,
    TitleBar
  }
}
</script>

<style scoped lang="stylus">
.home
  background #ffffff
</style>
