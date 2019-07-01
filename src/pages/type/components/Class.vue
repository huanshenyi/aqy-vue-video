<template>
 <div>
   <div class="class-top">
      <div>
        <section class="section-text">大型ペット</section>
      </div>
      <div class="class-content">
        <section>
          <a class="m-list-link" v-for="item in typelist" :key="item.id">
            <i class="listicon" :style="{backgroundPosition:item.size}"></i>
            <span class="list-info">{{item.text}}</span>
          </a>
        </section>
      </div>
      <div class="footer">
        <img src="//www.iqiyipic.com/common/fix/h5-aura/foot.png" alt="">
      </div>
   </div>
 </div>
</template>

<script>
export default {
  name: 'Class',
  data () {
    return {
      typelist: [{
        id: '001',
        size: '0 0',
        text: 'ワンちゃん'
      }, {
        id: '002',
        size: '-5rem 0',
        text: 'にゃんこ'
      }, {
        id: '003',
        size: '-15rem 0',
        text: 'ワンちゃん'
      }, {
        id: '004',
        size: '-10rem 0',
        text: 'ワンちゃん'
      }, {
        id: '005',
        size: '-25rem -25rem',
        text: 'ワンちゃん'
      }, {
        id: '006',
        size: '-10rem -5rem',
        text: 'ワンちゃん'
      }, {
        id: '007',
        size: '-20rem 0',
        text: 'ワンちゃん'
      }, {
        id: '008',
        size: '0 -5rem',
        text: 'ワンちゃん'
      }, {
        id: '009',
        size: '-5rem -5rem',
        text: 'ワンちゃん'
      }, {
        id: '010',
        size: '-15rem -5rem',
        text: 'ワンちゃん'
      }]
    }
  }
}
</script>

<style scoped lang="stylus">
.class-top
  background-color #fff
  .section-text
   padding-left 1.5rem
   line-height 2rem
   background-color #f7f7f7
   color #999
   font-size 1rem
  .class-content
   padding-left 0
   padding-right 0
   .m-list-link
    display inline-block
    vertical-align top
    width 32%
    height 6.8rem
    text-align center
    margin-top 1rem
    .listicon
     display inline-block
     width 5rem
     height 5rem
     background url("//www.iqiyipic.com/common/fix/h5-aura/channel-list-20190115.png")
     background-repeat no-repeat
     background-size 30rem 35rem
     background-position 0 0
    .list-info
     display block
     color #666
.footer
 padding 1.5rem
 text-align center
.footer img
  width 10rem
  height 4.7rem
</style>
