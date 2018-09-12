<template>
    <div class="n_input">
        <input :type="type" :placeholder="placeholder">
    </div>
</template>
<script>
    export default {
        name:'Ninput',
        props:{
            type:{
                default:'text',
                type:String
            },
            placeholder:{
                default:'请输入内容',
                type:String
            }
        }
    }
</script>

<style lang="stylus">
div.n_input
    display inline-block
    line-height 1px
    font-size 16px
    width 100%
    height 36px
    input
        border 1px solid #ebebeb
        width 100%
        padding 8px 10px
        box-sizing border-box
        outline none 
        background-image none 
        -webkit-appearance none
        font-size inherit
</style>