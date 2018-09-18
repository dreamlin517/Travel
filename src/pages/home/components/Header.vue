<template>
  <div class="header">
    <div class="left">
        <span class="iconfont back">&#xe622;</span>
    </div>
    <div class="input">
        <span class="iconfont seek">&#xe6de;</span>
        <input class="sou" type="text" placeholder="景点\门票">
    </div>
    <div class="right">城市
        <span class="iconfont san">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.header
    display: flex
    line-height: .86rem
    background: #00bcd4
    color: #fff
    
    .left
        width: .64rem
        .back
            position:relative
            left: 8px
    .input
        flex:1
        border-radius:5px
        position:relative
        .sou
            height:.64rem
            width: 4.36rem
            background:#fff
            border-radius: 5px
            margin-left:5px
            margin-right:5px
            padding-left:18px
            padding-right:4px
            font-size: 12px
            position:absolute
            bottom:6px
            right:5px
        .seek
            float:left 
            color:black 
            position:absolute
            left:3px
            top:1px
            z-index:2

    .right
        width: 1.24rem
        .san
            font-size: 12px

</style>