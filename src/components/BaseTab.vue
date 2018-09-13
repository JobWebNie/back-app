<template>
    <div class="">
        <div class="n_tabbar">
            <a class="n_tab_item block" href="#">
                <div class="n_tab_item_icon">
                    <slot name="icon"></slot>
                </div>
                <div class="n_tab_item_name">
                    <slot>
                    </slot>
                </div>
            </a>
        </div>
    </div>
</template>
<script>

    export default {
        name:'NBaseslot',
         components: {
        },
        props:{
               icon:{
                default:'../assets/images/1.png',
                type:String
            },
            title:{
                default:'这是商品名称',
                type:String
            },
            desc:{
                default:'这是一段描述性文字',
                type:String
            }
        },
        data(){
            return{
            }
        }
    }
</script>

<style lang="stylus">
@import '../assets/styl/base.styl'
div.n_tabbar
    position fixed
    bottom 0
    left 0
    right 0
    z-index 1
    display flex
    a.n_tab_item
        margin 8px 0
        flex 1
        .n_tab_item_icon
            height 24px
            width 24px
            margin 0 auto 5px
            img
                height 100%
                width 100%
        .n_tab_item_name
            font-size 12px
            text-align center
</style>