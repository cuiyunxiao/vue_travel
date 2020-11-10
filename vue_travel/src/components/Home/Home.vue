<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-location></home-location>
    <home-activity></home-activity>
    <home-live></home-live>
     <home-weekend></home-weekend>
  </div>
</template>

<script>
  import HomeHeader from './pages/Header'
  import HomeSwiper from './pages/Swiper'
  import HomeIcons from './pages/Icons'
  import HomeLocation from './pages/Location'
  import HomeActivity from './pages/Activity'
  import HomeHot from './pages/Hot'
  import HomeLive from './pages/Live'
  import HomeWeekend from './pages/Weekend'
  export default {
    components: {
      HomeHeader,
      HomeSwiper,
      HomeIcons,
      HomeLocation,
      HomeActivity,
      HomeHot,
      HomeLive,
      HomeWeekend
    }
  }
</script>

<style>
</style>
