<template>
  <div class="star">
    <div class="cc-title">
      <h1 class="hsico">参加者</h1>
      <svg class="icon">
        <use xlink:href="#icon-youjiantou"></use>
      </svg>
    </div>
    <div class="icons">
      <swiper :options="swiperOption">
        <swiper-slide v-for="(page, index) in pages" :key="index">
          <a class="star-big" v-for="item in page" :key="item.id">
            <span class="star-img" :style="{backgroundImage:'url('+item.Image+')'}"></span>
            <span class="star-center">{{item.text}}</span>
          </a>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Star',
  data () {
    return {
      swiperOption: {},
      starlist: [{
        id: '001',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }, {
        id: '002',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }, {
        id: '003',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }, {
        id: '004',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }, {
        id: '005',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }, {
        id: '006',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }, {
        id: '007',
        Image: 'https://or-formation.com/uploads/img/produits/46.png',
        text: 'python同好会'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.starlist.forEach((item, index) => {
        const page = Math.floor(index / 4)
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
.star
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
   margin-top 1.5rem
   border-bottom 1px solid #f0f0f0
   .star-big
    display inline-block
    width 25%
    height auto
    text-align center
    .star-img
     display inline-block
     width 60%
     padding-top 43%
     background-image url("https://or-formation.com/uploads/img/produits/46.png")
     background-repeat no-repeat
     background-size 100%
     border-radius: 50%
    .star-center
     display block
     height 3rem
     line-height 2rem
     overflow hidden
     text-overflow ellipsis
     white-space nowrap
     font-size 1rem
     color #333
</style>
