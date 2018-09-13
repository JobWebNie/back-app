<template>
    <div class="n_tabbar">
       <slot></slot>
    </div>
</template>
<script>
export default {
  name: 'app',
  props: {
    value: {}
  }
}
</script>

<style lang="stylus">
div.n_tabbar
    position fixed
    bottom 0
    left 0
    right 0
    z-index 1
    display flex
    
</style>
