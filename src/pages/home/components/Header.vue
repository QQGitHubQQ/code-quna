<template>
    <div class="header">
        <div class="header-left">
             <div class="iconfont icon-1">&#xe622;</div>
        </div>
        <div class="header-input">
            <span class="iconfont icon-2">&#xe623;</span>
            输入城市</div>
        <div class="header-right">城市
            <span class="iconfont icon-3">&#xe60c;</span>
        </div>
    </div>
</template>
<script>
export default {
    name:'Header'
}
</script>
<style lang="stylus">
 
    html,body{
        margin :0;
        padding :0;
    }
    .header
        display :flex
        background : #00bcd4
        line-height : 2.4rem /* 45/16 */
        .header-left 
            width : .64rem
            flex : 0.8
            float : left
            .icon-1
                font-size : 1.3rem
                text-align : center
        .header-input
            flex : 3
            border-radius : 5px
            background-color : #fff
            margin-top : .12rem
            margin-bottom : .12rem
            color: #ccc
            margin-left : .2rem
            .icon-2
                margin-left :.24rem
                font-size : 1.3rem
        .header-right 
            flex : 0.8
            width : 1.24rem
            text-align : center
            float : right
             

</style>
