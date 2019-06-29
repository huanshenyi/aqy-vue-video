<template>
<div class="icons">
 <swiper :options="swiperOption" v-if="list.length">
    <swiper-slide v-for="(list,index) of pages" :key="index">
       <div class="icons1" v-for="item of list" :key="item.id">
           <div class="icons-img">
            <img class="icons-imgsole" :src="item.imgUrl">
            <p class="icon-text">{{item.desc}}</p>
           </div>
       </div>
    </swiper-slide>
</swiper>
</div>
</template>

<script>

export default{
  name: 'HomeTubiao',
  data: function () {
    return {
      swiperOption: {},
      list: [{
        'id': '0001',
        'imgUrl': 'http://m.iqiyipic.com/common/lego/20170921/3ba9004a0a1e43939cf4631a5f0b8c8f.png',
        'desc': 'ドラマ解説'
      }, {
        'id': '0002',
        'imgUrl': 'http://m.iqiyipic.com/common/lego/20170915/7df91c03d5db4113848f7ca1b9d3f722.png',
        'desc': '小説解説'
      }, {
        'id': '0003',
        'imgUrl': 'http://m.iqiyipic.com/common/lego/20170915/bc4532a1bfd64f3c929b6f92002a57cd.png',
        'desc': '映画解説'
      }, {
        'id': '0004',
        'imgUrl': 'http://m.iqiyipic.com/common/lego/20180201/34b505af4dad4528a87cb15e2eb82f1c.png',
        'desc': '一般実況'
      }, {
        'id': '0005',
        'imgUrl': 'http://m.iqiyipic.com/common/lego/20170915/5909cbd78fd44f6fa3d9b78dc9e13cd2.png',
        'desc': 'ショップ'
      }, {
        'id': '0005',
        'imgUrl': 'http://m.iqiyipic.com/common/lego/20170915/5909cbd78fd44f6fa3d9b78dc9e13cd2.png',
        'desc': 'ショップ'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.list.forEach((item, index) => {
        const page = Math.floor(index / 5)
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

<style lang="stylus" scoped>
.icons
 background #ffffff
 margin-top:.5rem
 .icons1
  position:relative
  float:left
  width:20%
  padding-bottom:21%
  text-align:center
  .icons-img
   display:inline-block
   position:absolute
   top:0
   left:0
   bottom:1.2rem
   padding:1rem
   .icons-imgsole
    height:100%
   .icon-text
    margin-top:.5rem
    height:.5rem
    color:#333
</style>
