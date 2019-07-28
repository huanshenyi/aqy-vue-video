<template>
    <div class="pinglun">
      <div class="pinglun_dj">
           <div class="pinglun_border">
              <div class="pinglun_pin">
                <svg class="icon">
                  <use xlink:href="#icon-pinglun1"></use>
                </svg>
                <i class="pinglun_lnk">コメントを書く</i>
              </div>
           </div>
      </div>
      <div class="sixo">
        <div class="c-title">
          <div class="hsicoss">コメント</div>
          <span class="hsica">(37)</span>
        </div>
      </div>
      <div class="pinglun_centent">
        <div class="pinglun_top">
          <div class="pinglun_left">
             <div class="c-photo"></div>
             <div class="info">
               <div></div>
             </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Comment'
}
</script>

<style scoped lang="stylus">
.pinglun
  margin-top 2rem
  .pinglun_dj
   width 100%
   height 1rem
   position relative
   .pinglun_border
    position absolute
    width 90%
    height 3rem
    left 50%
    transform translate(-50%,-50%) //中間集中
    .pinglun_pin
     width 100%
     height 3rem
     line-height 3rem
     border-radius 1.5rem
     background #f5f5f5
     font-size 1.5rem
     text-align center
     .icon
        width: 1em;
        height: 1em;
        vertical-align: -0.15em;
        fill: currentColor;
        overflow: hidden;
     .pinglun_lnk
      color #87cefa
      font-size 1.3rem
      margin-left .5rem
  .sixo
   margin-top 1rem
   .c-title
    height 2rem
    line-height 2rem
    color #333
    margin-left 1rem
    position relative
    .hsicoss
      position absolute
      font-weight bold
      font-size 1.1rem
    .hsica
     margin-left 5rem
  .pinglun_centent
   position relative
   margin-top 1.5rem
   padding-bottom .3rem
   .pinglun_top
    padding 0 1.2rem .5rem 1.2rem
    .pinglun_left
     width 85%
     .c-photo
      width 3.5rem
      height 3.5rem
      border-radius 2rem
      background-image:url("https://s3-ap-northeast-1.amazonaws.com/petpedia/upload_by_admin/hedgehog_breeding_800.jpg")
      background-size cover
</style>
