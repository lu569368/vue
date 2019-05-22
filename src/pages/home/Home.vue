<template>
   <div>
      <home-header></home-header>
      <home-swiper></home-swiper>
      <home-icont></home-icont>
   </div>
</template>
<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcont from './components/Icont'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcont
  }
}
</script>
<style>
</style>
