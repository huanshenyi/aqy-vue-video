<template>
    <div>
      <div class="zt">
        <video id="example_video_1" class="video-js vjs-default-skin b" controls preload-eventes="none"
               poster="http://vjs.zencdn.net/v/oceans.png" data-setup="{}">
          <source src="http://vjs.zencdn.net/v/oceans.mp4" type="video/mp4">
        </video>
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
</style>
