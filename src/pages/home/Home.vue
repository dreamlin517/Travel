<template>
  <div>
    <HomeHeader></HomeHeader> 
    <HomeSwiper></HomeSwiper>
  </div>
</template>

<script>
import HomeHeader from './components/Header';
import HomeSwiper from './components/Swiper';

export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
