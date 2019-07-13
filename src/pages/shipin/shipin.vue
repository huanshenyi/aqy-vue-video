<template>
 <div class="home">
   <home-header></home-header>
   <fa-slo></fa-slo>
   <home-footer></home-footer>
 </div>
</template>

<script>
import HomeHeader from '../home/components/Header'
import FaSlo from './components/faslo'
import HomeFooter from '../home/components/Footer'
export default {
  name: 'shipin',
  components: {
    HomeHeader,
    FaSlo,
    HomeFooter
  }
}
</script>

<style scoped lang="stylus">
.home
  background #ffffff
</style>
