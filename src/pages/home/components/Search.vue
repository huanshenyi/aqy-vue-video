<template>
    <div>
      <div class="setop"></div>
      <div class="only_search">
        <div class="m-search">
          <div class="config_search">
             <span class="center">pythonナイス</span>
               <a href="" class="ziti">
                  <svg class="icon">
                     <use xlink:href="#icon-fangdajing"></use>
                  </svg>
               </a>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeSearch'
}
</script>

<style scoped lang="stylus">
  .setop
    background #ffffff
    height:2.9rem
  .only_search
    height 2.9rem
    background #F6F6F6
    position relative
    .m-search
     position absolute
     width 90%
     height 2rem
     left 50%
     top:50%
     transform translate(-50%,-50%)
     .config_search
      width 100%
      height 100%
      border-radius 1.5rem
      border 1px solid #87cefa
      background #FFF
      .center
       display block
       margin-right 5rem
       overflow hidden
       line-height 2rem
       text-align center
       font-size .9rem
       color #666
      .ziti
        display block
        position absolute
        top:.04rem
        right -.2rem
        width 4rem
        height 2rem
        background #87cefa
        border-bottom-right-radius 1.5rem
        border-top-right-radius 1.5rem
        .icon
          position relative
          display inline-block
          line-height 1.9rem
          left 50%
          top 50%
          transform translate(-50%,-50%)
          width: 1.9em;
          height: 1.9em;
          vertical-align: -0.15em;
          fill: currentColor;
          overflow: hidden;
</style>
