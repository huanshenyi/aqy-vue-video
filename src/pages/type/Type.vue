<template>
    <div class="type">
      <home-header></home-header>
      <class></class>
<!--      <home-footer></home-footer>-->
      <bottom-nav></bottom-nav>
    </div>
</template>

<script>
import HomeHeader from '../home/components/Header'
import Class from './components/Class'
// import HomeFooter from '../home/components/Footer'
import BottomNav from './components/Bottomnav'

export default {
  name: 'Type',
  components: {
    HomeHeader,
    Class,
    // HomeFooter
    BottomNav
  }
}
</script>

<style scoped lang="stylus">
.type
  background #ffffff
</style>
