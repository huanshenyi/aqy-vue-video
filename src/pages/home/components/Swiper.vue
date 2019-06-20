<template>
    <div class="lunbo">
        <swiper :options="swiperOption">
            <swiper-slide v-for="( page,index) in pages" :key="index">
              <div class="swiperNBA">
                <a href="" class="a_img" v-for="list of page" :key="list.id"
                   :style="{backgroundImage:'url('+list.Image+')'}">
                  <span class="images-left">{{list.text}}</span>
                  <span class="images-right">{{list.time}}</span>
                  <div>
                    <i class="text_img" :style="{backgroundPosition:list.size}"></i>
                  </div>
                </a>
              </div>
            </swiper-slide>
        </swiper>
    </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {},
      textList: [{
        id: '001',
        Image: 'https://img.capitalwatch.com/201902/13/5c64d088d45b0.jpg',
        text: 'The Wandering Earth',
        time: '上映中',
        size: '-4rem 0'
      }, {
        id: '002',
        Image: 'https://originalnews.nico/wp-content/uploads/2017/07/1002.jpg',
        text: 'オワコン',
        time: '実況中',
        size: '-4rem 0'
      }, {
        id: '003',
        Image: 'https://i.ytimg.com/vi/0ZNYL0aZU4s/maxresdefault.jpg',
        text: '快適な車中泊',
        time: '実況中',
        size: '-4rem 0'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.textList.forEach((item, index) => {
        const page = Math.floor(index / 1)
        if (!pages[page]) {
          pages[page] = []
        }
        pages[page].push(item)
      })
      return pages
    }
  }
}
</script>

<style scoped lang="stylus">
  .lunbo
   margin-top .5rem
   .swiperNBA
    width 100%
   .a_img
    display :block
    position relative
    width 100%
    padding-bottom 50%
    background-image :url("https://img.capitalwatch.com/201902/13/5c64d088d45b0.jpg")
    background-size 100% 100%
   .a_img:after
    position absolute
    left 0
    right 0
    bottom 0
    content ""
    height 3rem
    background-image linear-gradient(to bottom,rgba(0,0,0,0)0,rgba(0,0,0,0.5) 100%)
   .images-left
     display block
     position absolute
     left 0
     bottom 0
     height 3rem
     line-height 3rem
     color #FFF
     font-weight bold
     font-size 1rem
     z-index 50
     padding-left 1.1rem
    .images-right
      display block
      position absolute
      right  0
      bottom 0
      height 3rem
      line-height 3rem
      color #FFF
      z-index 50
      padding-right  1.1rem
    .text_img
     display inline-block
     position absolute
     width 3.5rem
     height 1.5rem
     background url("http://www.iqiyipic.com/common/fix/h5-aura/picicon-bg-20181205.png")
     background-repeat no-repeat
     background-size 15rem 15rem
     background-position -4rem 0
     right 0
</style>
