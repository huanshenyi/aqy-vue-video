<template>
    <div class="header">
      <div class="m-header header-fiexd">
        <img class="a-header b-header c-header" src="../../../../static/video-vue.png"/>
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
 height: 4.4 rem
 .m-header
     height 4.4rem
     background #F0FFFF
 .header-fiexd
     position fiexd
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
      top: 1rem
      left 1.2rem
     .mush
      padding-inline-start 10 px
      height 100%
      font-size 1.4rem
      float right
     .mush>li
      display inline-block
      width 3rem
      height 4.4rem
      text-align :center
      float left
      .icon
        display inline-block
        width: 1em;
        height: 1em;
        line-height 4.4rem
     .twoinfo
        float right
        height 4.4rem
        line-height 4.4rem
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
