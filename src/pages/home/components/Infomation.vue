<template>
    <div>
      <div class="box-conter">
        <div class="box-header">
          <a href="">
            <svg class="icon" aria-hidden="true">
              <use xlink:href="#icon-zujian-dibudaohang"></use>
            </svg>
            <div class="info-text">本日のおすすめ</div>
          </a>
        </div>
      </div>
      <div class="box-left">
        <div class="box-bottom">
          <div class="m-text">
            <svg class="icon">
              <use xlink:href="#icon-bofang"></use>
            </svg>
            <span class="text-child">8歳現役小学生アイドル</span>
          </div>
          <div class="m-text">
            <svg class="icon">
              <use xlink:href="#icon-bofang"></use>
            </svg>
            <span class="text-child">8歳現役小学生アイドル</span>
          </div>
        </div>
      </div>
      <div class="pic-content">
            <a class="a-content" v-for="item in infolist" :key="item.id">
              <div class="mic-img" :style="{backgroundImage:'url('+item.Image+')'}"></div>
              <div class="mic-text">{{item.text}}</div>
            </a>
      </div>
      <div style="clear: both"></div>
      <div class="end">
        <a class="a_left"><i class="iconfont fontfamily">&#xe627;</i>もっと</a>
        <a class="a_left"><i class="iconfont fontfamily">&#xe61c;</i>更新</a>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeInfomation',
  data () {
    return {
      infolist: [{
        id: '001',
        Image: 'https://s3-ap-northeast-1.amazonaws.com/petpedia/upload_by_admin/hari-01_800.jpg',
        text: 'ハリネズミ可愛い'
      }, {
        id: '002',
        Image: 'https://s3-ap-northeast-1.amazonaws.com/petpedia/upload_by_admin/hari-01_800.jpg',
        text: 'ハリネズミ可愛い'
      }]
    }
  }
}
</script>

<style scoped lang="stylus">
.box-conter
  border-top:1px solid #F0F0F0
  .box-header
    position relative
    padding: .1rem 1.2rem
    .icon
      width: 2 rem;
      height: 2 rem;
    .info-text
     color #333
     font-size 1.1rem
     display inline-block
     position relative
     line-height 1.5rem
     max-width:70%
     font-weight bold
.box-left
  padding-left 1rem
  .box-bottom
   padding-bottom 1rem
   .m-text
    position relative
    line-height 1rem
    margin-bottom .15rem
    padding  0 .12rem 0 .31rem
    .icon
       width: 1.5 rem;
       height: 1.5 rem;
    .text-child
     color #333
     font-size 1.1rem
.pic-content
 margin-left -.2rem
 .a-content
  display inline-block
  width 49.5%
  height auto
  float left
  .mic-img
   width 100%
   padding-bottom 50%
   background-image :url("https://s3-ap-northeast-1.amazonaws.com/petpedia/upload_by_admin/hari-01_800.jpg")
   background-size cover
   position relative
  .mic-text
   padding-top 0.5rem
   padding-left 1rem
   color #333
   font-size 1.1rem
   line-height 2rem
.end
 height 5rem
 .a_left
  display inline-block
  width 49%
  color :#0bbe06
  text-align center
  line-height 1.5rem
  font-size 1.1rem
  .fontfamily
   margin-left .5rem
</style>
