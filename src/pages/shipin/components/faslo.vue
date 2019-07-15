<template>
    <div>
      <div class="zt">
         <div>
          <video id="example_video_1" class="video-js vjs-default-skin b vjs-big-play-centered" controls preload-eventes="none"
               poster="//www.iqiyipic.com/common/fix/h5-v3/player-tip-bg.jpg" data-setup="{}">
           <!--poster="//www.iqiyipic.com/common/fix/h5-v3/player-tip-bg.jpg" defaultの画像-->
           <source src="http://vjs.zencdn.net/v/oceans.mp4" type="video/mp4">
          </video>
       </div>
      </div>
      <div class="bottom_kj">
        <div class="bottom_centent">
          <a class="a_centent">
            <svg class="icon">
              <use xlink:href="#icon-bofang"></use>
            </svg>
            アプリをゲット、三倍速を体験
          </a>
        </div>
      </div>
      <div class="pinlun">
         <section class="pinlun_content">
           <div class="pinlun_left">
             <svg class="icon">
               <use xlink:href="#icon-pinglun2"></use>
             </svg>
               <span class="pic-text">4,233</span>
           </div>
           <div class="pinlun_right">
              <div class="xiazai">
                <svg class="icon">
                  <use xlink:href="#icon-xiazailan"></use>
                </svg>
              </div>
             <div class="xiazai">
               <svg class="icon">
                 <use xlink:href="#icon-fenxiang1"></use>
               </svg>
             </div>
             <div class="xiazai">
               <svg class="icon">
                 <use xlink:href="#icon-gengduo"></use>
               </svg>
             </div>
           </div>
         </section>
      </div>
    </div>
</template>

<script>
export default {
  name: 'faslo'
}
</script>

<style scoped lang="stylus">
.zt
  position relative
  padding-top 52.25%
  .b//videoのサイズ
    position absolute
    top 0
    right 0
    bottom 0
    width 100%
    height 100%
.bottom_kj
  height 3rem
  margin-top .5rem
  position relative
  .bottom_centent
   position absolute
   width 90%
   height 3rem
   left 50%
   top 50%
   transform translate(-50%,-50%)
   .a_centent
     color #ffffff
     display block
     position relative
     width 100%
     height 2.5rem
     line-height 2.5rem
     border-radius 2rem
     border 1px solid #87cefa
     background-image linear-gradient(to right,#87cefa 0,#007aff 100%)
     text-align center
     .icon
      position relative
      width: 1.5em;
      height: 1.5em;
      vertical-align: -0.4em;
      fill: currentColor;
      overflow: hidden;
      margin-right 0.1rem
.pinlun
  height 3.5rem
  margin-top 0.5rem
  .pinlun_content
   position relative
   height 3rem
   border-bottom 1px solid #f0f0f0
   .pinlun_left
    position relative
    width 40%
    margin 0 1rem 0 1rem
    float left
    .icon
     display inline-block
     width 2rem
     height 2rem
    .pic-text
     font-size: 14px
     position absolute
     margin-top .6rem
     margin-left .5rem
   .pinlun_right
    width 50%
    float right
    text-align right
    .xiazai
      display inline-block
      width 3rem
      text-align center
     .icon
       width: 2em;
       height: 2em;
       fill: currentColor;
       overflow: hidden;
</style>
