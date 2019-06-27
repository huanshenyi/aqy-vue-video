<template>
    <div class="pic-content">
      <a class="a-content" v-for="item in Listcontent" :key="item.id">
        <div class="mic-img" :style="{backgroundImage:'url('+item.Image+')'}">
          <span class="mix-text">{{item.text}}</span>
        </div>
        <div class="mic-text">
          <div class="pic-p">{{item.name}}</div>
          <div class="mic-p">{{item.conent}}</div>
        </div>
      </a>
    </div>
</template>

<script>
export default {
  name: 'HomeList',
  data () {
    return {
      Listcontent: [{
        id: '0001',
        Image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg',
        text: '実況中',
        name: 'ハリネズミの日常',
        conent: 'シュシュシュ'
      }, {
        id: '0002',
        Image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg',
        text: '実況中',
        name: 'ハリネズミの日常',
        conent: 'シュシュシュ'
      }, {
        id: '0003',
        Image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg',
        text: '実況中',
        name: 'ハリネズミの日常',
        conent: 'シュシュシュ'
      }, {
        id: '0004',
        Image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg',
        text: '実況中',
        name: 'ハリネズミの日常',
        conent: 'シュシュシュ'
      }, {
        id: '0005',
        Image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg',
        text: '実況中',
        name: 'ハリネズミの日常',
        conent: 'シュシュシュ'
      }, {
        id: '0006',
        Image: 'https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg',
        text: '実況中',
        name: 'ハリネズミの日常',
        conent: 'シュシュシュ'
      }]
    }
  }
}
</script>

<style scoped lang="stylus">
  .pic-content
   margin-left :-.2rem
   margin-top 0.5rem
   .a-content
    display inline-block
    width 49.5%
    height auto
    margin-left .1rem
    .mic-img
     width 100%
     padding-bottom 50%
     background-image :url("https://cdn-ak.f.st-hatena.com/images/fotolife/c/chikojirou/20161227/20161227212323.jpg")
     background-size cover
     position relative
     .mix-text
      display block
      height 1rem
      line-height 1rem
      position absolute
      bottom 0
      right 0
      padding-right 0.8rem
      color #fff
      z-index 100
    .mic-text
      padding-left 1rem
      .pic-p
       padding-top 0.5rem
       font-size 1rem
       color #333
       display block
       height 1rem
      .mic-p
       font-size 1rem
       height 1.5rem
       line-height 1.5rem
       margin-bottom 0.5rem
    .mic-img:after
     position absolute
     left 0
     right 0
     bottom 0
     content ""
     height 3rem
     background-image :linear-gradient(top,rgba(0,0,0,0)0,rgba(0,0,0,0.5)100%)
</style>
