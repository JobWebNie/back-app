<template>
    <div class="n_flexbox">
        <a class="n_item block mr-2" href="#">
            <div class="n_item_name">这是商品名称</div>
            <p class="n_item_desc">这是一段描述性文字</p>
        </a>
    </div>
</template>
<script>
    export default {
        name:'Flexbox',
        props:{
            // type:{
            //     default:'text',
            //     type:String
            // },
            // placeholder:{
            //     default:'请输入内容',
            //     type:String
            // }
        }
    }
</script>

<style lang="stylus">
@import '../../assets/styl/base.styl'
div.n_flexbox
    float left
    margin-bottom 20px
    margin-right 10px
    a:hover
        box-shadow 0 0 6px #ebebeb
        transform translateY(-2px)
    a:active
        background-color #ebebeb
        transform translateY(-2px)
.n_item
    background-color #ffffff
    box-sizing border-box
    .n_item_name
        color #333333
        font-size 16px
        text-align left 
        line-height 32px
    .n_item_desc
        color #666666
        font-size 12px
        line-height 24px
        margin 0px auto
</style>