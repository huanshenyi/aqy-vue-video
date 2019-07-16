<template>
    <div class="zhoubian">
      <div class="cc-title">
        <h1 class="hsico">関連動画</h1>
        <svg class="icon">
          <use xlink:href="#icon-youjiantou"></use>
        </svg>
      </div>
      <div class="icons">
        <swiper :options="swiperOption">
          <swiper-slide v-for="(page, index) in pages" :key="index">
            <a class="go-centent" v-for="item in page" :key="item.id">
              <div class="go-like" :style="{backgroundImage: 'url('+item.Image+')'}">
                   <span class="go-text">{{item.time}}</span>
              </div>
              <div class="go-app">
                 <span class="go-mic">{{item.text}}</span>
              </div>
            </a>
          </swiper-slide>
        </swiper>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Zhoubian',
  data () {
    return {
      swiperOption: {},
      list: [{
        id: '001',
        Image: 'https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg',
        time: '00:45',
        text: 'ハリネズミ居眠り'
      }, {
        id: '002',
        Image: 'https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg',
        time: '00:45',
        text: 'ハリネズミ居眠り'
      }, {
        id: '003',
        Image: 'https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg',
        time: '00:45',
        text: 'ハリネズミ居眠り'
      }, {
        id: '004',
        Image: 'https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg',
        time: '00:45',
        text: 'ハリネズミ居眠り'
      }, {
        id: '005',
        Image: 'https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg',
        time: '00:45',
        text: 'ハリネズミ居眠り'
      }, {
        id: '006',
        Image: 'https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg',
        time: '00:45',
        text: 'ハリネズミ居眠り'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.list.forEach((item, index) => {
        const page = Math.floor(index / 3)
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
  *{
    touch-action :none
  }
.zhoubian
  margin-top .5rem
  .cc-title
    height 2rem
    line-height 2rem
    color #333
    margin-left 1rem
    position relative
    .hsico
      position absolute
      font-weight bold
      font-size 1.1rem
    .icon
      width: 1.1em;
      height: 1.1em;
      position absolute
      right 2rem
  .icons
   margin-top .5rem
   border-bottom 1px solid #f0f0f0
   padding-bottom 1rem
   .go-centent
    display inline-block
    width 25%
    height auto
    margin-left 1.2rem
    .go-like
     width 90%
     padding-bottom 50%
     background-image url("https://static.pepy.jp/wp-content/uploads/2017/01/29014508/shutterstock_490940572.jpg")
     background-size cover
     position relative
     .go-text
      display block
      height 2rem
      line-height 2rem
      position absolute
      bottom 0
      right 0
      padding-right .5rem
      color #fff
      z-index 1000
    .go-like:after
      position absolute
      left 0
      right 0
      bottom 0
      content ""
      height 3rem
      background-image linear-gradient(top,rgba(0,0,0,0)0,rgba(0,0,0,0.5)100%)
    .go-app
      padding-top .3rem
      padding-left .3rem
     .go-mic
       color black
       height 1rem
       font-size .8rem
</style>
