<template>
        <a class="n_tab_item block"  :class="{ 'is_active': $parent.value === id }" @click.prevent="$parent.$emit('tapTabItem',id)" href="">
            <div class="n_tab_item_icon">
                <slot name="icon"></slot>
            </div>
            <div class="n_tab_item_name">
                <slot>
                </slot>
            </div>
        </a>
</template>
<script>
export default {
    name:'TabItem',
    props: ['id']
}
</script>
<style lang="stylus">
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
        color inherit
a.n_tab_item.is_active
    color #4cbaf1
</style>
