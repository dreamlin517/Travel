<template>
    <div>
            <div class="icons">
                <div class="icon">
                    <div class="icon-img">                     
                        <img class="icon-img-content" src="http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png" alt="">
                    </div>
                </div>
            </div>   
    </div>
</template>

<script>
    export default{
        name: 'HomeIcons',
    };
</script>

<style lang="stylus" scoped>
.icons
    overflow hidden
    height 0
    padding-bottom 50%
    width 100%
    background blue
    .icon
        overflow hidden
        position relative
        height 0
        padding-bottom 25%
        width 25%
        background red
        float left
        .icon-img
            width 100% 
            position absolute
            top 0
            right 0
            left 0 
            bottom .44rem
            background yellow
            text-align center
            line-height 100%
            .icon-img-content
                height   100%
                
</style>
