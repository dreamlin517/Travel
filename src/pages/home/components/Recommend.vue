<template>
    <div>
        <div class="title">热销推荐</div>
        <ul class="zus">
            <li class="zu" v-for = "item in recommendList" :key = "item.id" >
                <img class="pic" :src="item.imgUrl" alt="">
                <div class="pic-desc">{{ item.desc }}</div>
                <div class="pinjia">
                    <span class="iconfont">&#xe64a; &#xe64a;&#xe64a; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; 20065条评论</span>
                </div>
                <div class="pic-moeny">
                    <span class="moey">{{ item.moeny }}</span>
                    <span class="font">起</span>  
                    <span class="dre">{{ item.dre }}</span>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
    export default{
        name: 'HomeRecommend',
            data() {
                return {
                     recommendList: [
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '上海杜莎夫人蜡像馆',
                        moeny: '129',
                        dre: '黄浦区',
                        id: '0001',

                    },
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '大大大无无无',
                        moeny: '129',
                        dre: '浦东新区',
                        id: '0002',

                    },
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '粉色啊飒飒大',
                        moeny: '129',
                        dre: '黄浦区',
                        id: '0003',

                    },
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '的方式发顺丰',
                        moeny: '129',
                        dre: '黄浦区',
                        id: '0004',

                    },
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '法无法人跟人相处',
                        moeny: '129',
                        dre: '黄浦区',
                        id: '0005',

                    },
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '打的饭',
                        moeny: '129',
                        dre: '黄浦区',
                        id: '0006',

                    },
                    {
                        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
                        desc: '当时的说法是否',
                        moeny: '129',
                        dre: '黄浦区',
                        id: '0007',

                    },
                ],
                };
            },
    };
    
</script>

<style lang="stylus" scoped>
.title
    line-height .8rem
    background #eee
    text-indent .2rem  
    margin-top .2rem
.zus    
    width 100%
    box-sizing border-box
    height 0
    padding-bottom: 35%
    
    .zu
        padding 0 .2rem
        border-bottom 2px solid #ccc
        .pic
            width 35%
            height 100%
            float left
        .pic-desc
            padding  .44rem 0 .44rem 40%
        .pinjia 
            padding-left 40%
            .iconfont
                font-size 10px
        .pic-moeny
            padding  .44rem 0 .44rem 40%
            .moey
                font-size 25px
                color yellow
            .font
                font-size 12px  
            .dre
                float right
                font-size 12px
            
</style>
