<template>
    <div class="type">
      <home-header></home-header>
      <class></class>
      <home-footer></home-footer>
    </div>
</template>

<script>
import HomeHeader from '../home/components/Header'
import Class from './components/Class'
import HomeFooter from '../home/components/Footer'

export default {
  name: 'Type',
  components: {
    HomeHeader,
    Class,
    HomeFooter
  }
}
</script>

<style scoped lang="stylus">
.type
  background #ffffff
</style>
