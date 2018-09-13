<template>
    <div class="n_flexbox two_part">
        <a v-for="(item,index) in listData" :key="item.id ? item.id : index" class="n_item block" href="#">
            <div class="n_item_icon">
                <img :src="item.icon" alt="商品图片">
            </div>
            <div class="n_item_info">
                <div class="n_item_name">{{item.title}}</div>
                <p class="n_item_desc">{{item.desc}}</p>
            </div>
        </a>
        <!-- <a class="n_item block" href="#">
            <div class="n_item_icon">
                <img src="../../assets/images/1.png" alt="商品图片">
            </div>
            <div class="n_item_info">
                <div class="n_item_name">这是商品名称</div>
                <p class="n_item_desc">这是一段描述性文字</p>
            </div>
        </a> -->
    </div>
</template>
<script>
    export default {
        name:'Flexbox',
        props:{
            listData:{
                default: null,
                type: Array
            }
            // icon:{
            //     default:'text',
            //     type:String
            // },
            // title:{
            //     default:'这是商品名称',
            //     type:String
            // },
            // desc:{
            //     default:'这是一段描述性文字',
            //     type:String
            // }
        }
    }
</script>

<style lang="stylus">
@import '../../assets/styl/base.styl'
div.n_flexbox
    margin-bottom 20px
    a:hover
        box-shadow 0 0 6px #ebebeb
        transform translateY(-2px)
    a:active
        background-color #ebebeb
        transform translateY(-2px)
div.two_part
    display flex
    .n_item
        width 50%
        &:nth-child(2n-1)
            margin-right 10px
.n_item
    background-color #ffffff
    box-sizing border-box
    margin-bottom 10px
    .n_item_name
        color #333333
        font-size 16px
        text-align center
        line-height 32px
    .n_item_desc
        color #666666
        font-size 12px
        text-align center 
        line-height 24px
        margin 0px auto
.n_item.horizon
    display flex 
    .n_item_icon
        width 80px
        img
            width 100%
            box-sizing border-box
    .n_item_name
        text-align left 
    .n_item_desc
        text-align left
</style>