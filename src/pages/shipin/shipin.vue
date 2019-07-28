<template>
 <div class="home">
   <home-header></home-header>
   <fa-slo></fa-slo>
   <title-bar></title-bar>
   <mu-lu></mu-lu>
   <zhou-bian></zhou-bian>
   <star></star>
   <comment></comment>
<!--   <home-footer></home-footer>-->
 </div>
</template>

<script>
import HomeHeader from '../home/components/Header'
import FaSlo from './components/faslo'
import TitleBar from './components/Titlebar'
import MuLu from './components/Mulu'
import ZhouBian from './components/Zhoubian'
import Comment from './components/Comment'
// import HomeFooter from '../home/components/Footer'
import Star from './components/Star'
export default {
  name: 'shipin',
  components: {
    HomeHeader,
    FaSlo,
    // HomeFooter,
    TitleBar,
    MuLu,
    ZhouBian,
    Star,
    Comment
  }
}
</script>

<style scoped lang="stylus">
.home
  background #ffffff
</style>
