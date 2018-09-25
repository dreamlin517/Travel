<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for = "item of SwiperList" :key="item.id" >
                <img :src=" item.imgUrl " alt="">
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
  </div>

</template>
     
<script>
    export default{
        name: 'HomeSwiper',
        data() {
      return {
        swiperOption: {
            pagination: '.swiper-pagination',
            loop: true,
        },
        SwiperList: [{
            id: '0001',
            imgUrl: 'http://img1.qunarzz.com/piao/fusion/1807/66/e5a5cec881702f02.jpg_750x200_67bb5691.jpg',
        },
        {
            id: '0002',
            imgUrl: 'http://img1.qunarzz.com/piao/fusion/1809/cd/a0acbb1831b18402.jpg_750x200_00d2cd78.jpg',
        },
        {
            id: '0003',
            imgUrl: 'http://img1.qunarzz.com/piao/fusion/1809/9b/8f79dbd1e0941302.jpg_750x200_55829659.jpg',
        },
        ],
      };
    },
    };
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background #fff
.wrapper
    width 100%
    height 0
    padding-bottom 26.6% 
    overflow hidden
    img
        width 100%

</style>
