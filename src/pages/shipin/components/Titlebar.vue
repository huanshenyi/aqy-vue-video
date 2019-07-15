<template>
  <div class="m-box">
     <div>
       <div class="m-video-info">
         <a style="color: #000000">
           <h1 class="c-title">python車中泊:pat1</h1>
           <svg class="icon">
             <use xlink:href="#icon-youjiantou"></use>
           </svg>
         </a>
         <a class="a-js">
           <svg class="icon">
             <use xlink:href="#icon-redu"></use>
           </svg>
           <div class="span_left">Hot:6675</div>
           <div class="span_center">5分前UP</div>
           <div class="span_right">Python愛好会連合会</div>
         </a>
       </div>
     </div>
  </div>
</template>

<script>
export default {
  name: 'TitleBar'
}
</script>

<style lang="stylus" scoped>
.m-box
  padding-left 0
  padding-right 0
  border-bottom 1px solid #f0f0f0
  padding-bottom .5rem
  .m-video-info
   padding 0 .12rem .15rem .12rem
   .c-title
    font-weight bold
    float left
    font-size 1.4rem
    color #333
    margin-left 1rem
   .icon
     width: 1.5em;
     height: 1.5em;
     vertical-align: -0.15em;
     fill: currentColor;
     overflow: hidden;
     margin-left 7rem
   .a-js
    display block
    width 100%
    height 3rem
    line-height 3rem
    margin-top .5rem
    .icon
      width: 2em;
      height: 2em;
      margin-left .5rem
      display inline-block
      float left
      padding-top .5rem
    .span_left
     float left
     color #999
     font-size 1.1rem
     margin-left .2rem
    .span_center
      float left
      color #999
      font-size 1.1rem
      margin-left .5rem
    .span_right
      float right
      width 40%
      color #999
      font-size 1.1rem
      margin-left .5rem
      text-overflow ellipsis
      white-space nowrap
      overflow hidden
</style>
