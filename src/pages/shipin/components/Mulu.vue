<template>
    <div class="xuanji">
       <div class="cc-title">
           <h1 class="hsico">part選択</h1>
           <svg class="icon">
             <use xlink:href="#icon-youjiantou"></use>
           </svg>
       </div>
      <div class="partbar">
         <swiper :options="swiperOption">
           <swiper-slide v-for="page of pages" :key="page.id">
             <div class="icons1" v-for="item of page" :key="item.id">
               <div class="icons-img">{{item.text}}</div>
             </div>
           </swiper-slide>
         </swiper>
      </div>
    </div>
</template>

<script>
export default {
  name: 'MuLu',
  data () {
    return {
      swiperOption: {},
      mululist: [{
        id: '001',
        text: '1'
      }, {
        id: '002',
        text: '2'
      }, {
        id: '003',
        text: '3'
      }, {
        id: '004',
        text: '4'
      }, {
        id: '005',
        text: '5'
      }, {
        id: '006',
        text: '6'
      }, {
        id: '007',
        text: '7'
      }, {
        id: '008',
        text: '8'
      }, {
        id: '009',
        text: '9'
      }, {
        id: '010',
        text: '10'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.mululist.forEach((item, index) => {
        // console.log(item, index)
        const page = Math.floor(index / 6)
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
.xuanji
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
  .partbar
   margin-top .5rem
   border-bottom 1px solid #f0f0f0
   padding-bottom .5rem
   .icons1
    position relative
    float left
    width 3 rem
    height 3 rem
    text-align center
    background #fafafa
    margin-left .5rem
    .icons-img
     position absolute
     left 50%
     top 50%
     transform translate(-50%,-50%)
     color #333
     font-weight blod
</style>
