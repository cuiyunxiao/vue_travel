<template>
  <div>
 <home-header></home-header>
  <home-swiper></home-swiper>
 <home-icons></home-icons>
 <home-location></home-location>
 <home-activity></home-activity>
  <home-hot></home-hot>
  </div>
</template>

<script>
  import HomeHeader from './pages/Header'
  import HomeSwiper from './pages/Swiper'
  import HomeIcons from './pages/Icons'
  import HomeLocation from './pages/Location'
    import HomeActivity from './pages/Activity'
     import HomeHot from './pages/Hot'
    location
  export default{
    components:{
      HomeHeader,
      HomeSwiper,
      HomeIcons,
      HomeLocation,
      HomeActivity,
      HomeHot
    }
  }
</script>

<style>
</style>
