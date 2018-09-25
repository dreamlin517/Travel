<template>
    <div class="icons">
        <swiper :options="swiperOption">
            <swiper-slide v-for="(page, index) in pages" :key="index" >
                <div class="icon" v-for="item in page" :key="item.id">
                    <div class="icon-img">                     
                        <img class="icon-img-content" :src="item.imgUrl" alt="">
                        <p class="icon-img-desc">{{ item.desc }}</p>
                    </div>
                </div>
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>  
</template>

<script>
export default {
    name: 'HomeIcons',
    data() {
        return {
            swiperOption: {
                pagination: '.swiper-pagination',
                loop: true,
            },
            iconsList: [
                {
                    id: '001',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
                    desc: '景点门票',
                },
                {
                    id: '002',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
                    desc: '赏秋色',
                },
                {
                    id: '003',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png',
                    desc: '游乐场',
                },
                {
                    id: '004',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
                    desc: '上海必游',
                },
                {
                    id: '005',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
                    desc: '景点门票',
                },
                {
                    id: '006',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
                    desc: '赏秋色',
                },
                {
                    id: '007',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png',
                    desc: '游乐场',
                },
                {
                    id: '008',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
                    desc: '上海必游',
                },
                {
                    id: '009',
                    imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/47/c2b659e048b11602.png',
                    desc: '动物园',
                },
            ],
        };
    },
    computed: {
        pages() {
            const pages = [];
            this.iconsList.forEach((item, index) => {
                const page = Math.floor(index / 8);
                if (!pages[page]) {
                    pages[page] = [];
                }
                pages[page].push(item);
            });
            return pages;
        },
    },
};
</script>

<style lang="stylus" scoped>
.icons >>> .swiper-container {
    height: 0;
    padding-bottom: 50%;
    width: 100%;
}
.icons >>> .swiper-pagination-bullet-active
    background #fff

.icon {
    overflow: hidden;
    position: relative;
    height: 0;
    padding-bottom: 25%;
    width: 25%;
    float: left;

    .icon-img {
        width: 100%;
        position: absolute;
        top: 0;
        right: 0;
        left: 0;
        bottom: 0.44rem;
        text-align: center;
        line-height: 100%;

        .icon-img-content {
            height: 100%;
            position: relative;
            top: 0.08rem;
        }

        .icon-img-desc {
            margin: 0;
            box-sizing: border-box;
            padding-bottom: 0.44rem;
        }
    }
}
</style>
