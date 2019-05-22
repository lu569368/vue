<template>
  <div class="header">
    <div class='header-left'>
      <span class="iconfont">&#xe65b;</span>
    </div>
    <div class='header-input'>输入</div>
    <div class='header-right'>城市</div>
  </div>
</template>
<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang='stylus' scoped>
  @import '~styles/varibles.styl'
  .header
    display:flex
    line-height:.86rem
    background:$bgColor
    color:#fff
    .header-left
      width:.64rem
      float:left
      text-align:center
    .header-input
      flex:1
      height:.64rem
      line-height:.64rem
      margin-left:.2rem
      margin-top:.12rem
      background:#fff
      border-radius:.1rem
      color:#000
    .header-right
      width:1.24rem
      float:right
</style>
