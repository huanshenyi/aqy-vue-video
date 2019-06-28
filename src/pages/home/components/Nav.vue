<template>
    <div class="topNav">
      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-container"></div>
          <div class="swiper-slide  span-info">人気</div>
          <div class="swiper-slide" v-for="(swiperSlide,index) in swiperSlides" :key="index">{{swiperSlide}}</div>
        </div>
      </div>
      <div class="indexAdd">
        <img src="./img/nav-linebg.png">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-luntanzixun"></use>
        </svg>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeNav',
  data () {
    return {
      swiperSlides: ['描き', 'キャンプ', 'スポーツ', 'python', '成人', 'ドラマ', 'ニュース', '映画', 'ペット', 'キャンプ']
    }
  },
  mounted () {
    var mySwiper = new Swiper('.swiper-container', {
      slidesPerView : 5,
      slidesPerGroup : 6
    })
  }
}
</script>

<style scoped lang="stylus">
.topNav
  width 100%
  height 2.8rem
  position fixed
  line-height 2.8rem
  background #FFF
  border-bottom 1px solid #ccc
  z-index 1001
  .swiper-slide
    width 3rem
    color #333
    text-align center
    font-size 1rem
  .span-info
    color  #0bbe06
    font-weight:bold
  .span-info:before
   content ""
   position absolute
   left 50%
   bottom 0
   width 1rem
   height 0.2rem
   z-index 2
   transform translate(-50%,0)
   background #0bbe06
  .indexAdd
   position absolute
   right 0
   top 0
   width 3.6rem
   height 2.8rem
   text-align center
   z-index 5
   background #FFF
  .indexAdd>img
    position absolute
    left : -.05rem
    bottom 1rem
    top 0
    width 0.2rem
   .icon
    width: 2.6em;
    height: 2.8em;
</style>
