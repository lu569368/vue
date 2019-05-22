<template>
  <!-- 这块的意思是当用户的网速慢的时候容易出现轮播图还没有加载出来但是下面的文字加载出来了！这样写不会出现这种情况，下面的padding-botton是图片宽高的比 -->
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide>
        <img class="swiper-img" src="https://imgs.qunarzz.com/p/tts3/1807/35/f633ef70c3500a02.jpg_r_390x260x90_e32fd46c.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img class="swiper-img" src="https://imgs.qunarzz.com/p/tts9/1807/67/ca524c0ddc372302.jpg_r_390x260x90_be327f2e.jpg" alt="">
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
      <div class="swiper-scrollbar"   slot="scrollbar"></div>
    </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      }
    }
  }
}
</script>
<style lang="stylus" scoped>
  // scoped 只作用于当前的页面 swiper组件是main页面的注册组件，所有不能使用css>>>是穿透动画，不受当前页面限制
  .wrapper>>>.swiper-pagination-bullet-active
    background:#fff
    .wrapper
      overflow hidden
      width:100%
      height:0
      padding-bottom:30%
      background:#eee
      .swiper-img
        width 100%
        height 2.5rem
</style>
