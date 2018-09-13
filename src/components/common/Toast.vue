<template>
    <div class="n_toast">
        <!-- <slot><slot> -->
        <div class="n_toast_message">
            <img src="../../assets/images/check.png" alt="">
            <div class="n_toast_text">
                操作成功
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        name:'NToast',
        props:{
           
        }
    }
</script>
<style lang="stylus" scoped>
div.n_toast
    display flex
    position fixed
    top 0
    left 0
    right 0
    bottom 0
    color #ffffff
    align-items center
    .n_toast_message
        padding 20px
        background-color #4c4c4c;
        border-radius 4px
        margin 0 auto 
        width 100px
        img 
            width 100%
        .n_toast_text
            margin-top 20px
            font-size 16px
</style>