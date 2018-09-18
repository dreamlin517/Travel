<template>
  <div class="header">
    <div class="left">
        <span class="iconfont back">&#xe622;</span>
    </div>
    <div class="input">
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
        .sou
            height:.64rem
            width: 4.36rem
            background:#fff
            border-radius: 5px
            margin-left:5px
            margin-right:5px
            padding-left:8px
            padding-right:4px
            font-size: 12px
            
    .right
        width: 1.24rem
        .san
            font-size: 12px

</style>