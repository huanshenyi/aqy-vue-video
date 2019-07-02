<template>
    <div class="dinav">
      <div class="dinav_border a">
         <router-link to="/">
           <div class="inmei">
             <div class="cont">
               <i class="iconfont">&#xe626;</i>
             </div>
           </div>
         </router-link>
        <router-link to="/type">
          <div class="inmei">
            <div class="cont">
              <i class="iconfont">&#xe626;</i>
            </div>
          </div>
        </router-link>
        <router-link to="/">
          <div class="inmei">
            <div class="cont">
              <img src="../../../assets/logo.png" class="img-cen">
            </div>
          </div>
        </router-link>
        <router-link to="/">
          <div class="inmei">
            <div class="cont">
              <i class="iconfont">&#xe626;</i>
            </div>
          </div>
        </router-link>
        <router-link to="/">
          <div class="inmei">
            <div class="cont">
              <i class="iconfont">&#xe626;</i>
            </div>
          </div>
        </router-link>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Bottomnav'
}
</script>

<style scoped lang="stylus">
.dinav
  height 4.4rem
  .dinav_border
   position fixed
   left 0
   bottom 0
   right 0
   z-index: 1001
  .a
   height 4.4rem
   background  #fff
   .inmei
     display block
     width :20%
     height 4.4rem
     float left
     text-align center
     position relative
     .cont
      position absolute
      top:50%
      left 50%
      transform translate(-50%,-50%)
      .iconfont
        font-size 1.5rem
        color #999
      .content
        display block
        margin-top .3rem
      .img-cen
        height 4rem
</style>
