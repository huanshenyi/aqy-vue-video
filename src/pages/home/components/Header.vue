<template>
    <div class="header">
      <div class="m-header header-fiexd">
        <router-link to="/">
          <img class="a-header b-header c-header" src="../../../../static/video-vue.png"/>
        </router-link>
        <div class="twoinfo">
          <a class="line-text">Appゲット</a>
        </div>
        <ul class="mush">
          <li>
            <svg class="icon">
              <use xlink:href="#icon-fangdajing1"></use>
            </svg>
          </li>
          <li>
            <svg class="icon">
              <use xlink:href="#icon-_shizhong"></use>
            </svg>
          </li>
          <li>
            <svg class="icon">
              <use xlink:href="#icon-yonghu11"></use>
            </svg>
          </li>
        </ul>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
.header
 height: 3.5 rem
 .m-header
     height 3.5rem
     background #F0FFFF
 .header-fiexd
     position fixed
     top 0
     left 0
     right 0
     z-index 1001
     .a-header
      display inline-block
      width 7.3rem
      height 2.4rem
     .b-header
      background :image("../../../../static/video-vue.png") no-repeat 0 0
      background-size 7.3rem 2.4rem
     .c-header
      position absolute
      top: 0.5rem
      left 1.2rem
     .mush
      padding-inline-start 10 px
      height 100%
      font-size 1.2rem
      float right
      padding-right :1rem
     .mush>li
      display inline-block
      width 2rem
      height 3.5rem
      text-align :center
      float left
      .icon
        position: absolute
        display inline-block
        width: 1.2em;
        height: 1.2em;
        line-height 3.5rem
     .twoinfo
        float right
        height 3.5rem
        line-height 3.5rem
        margin-right .5rem
        .line-text
         display inline-block
         height 2rem
         line-height 2rem
         width 5rem
         border 1px solid #87CEFA
         border-radius 2rem
         text-align center
         font-size 1rem
         color #87CEFA
</style>
