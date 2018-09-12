<template>
    <div class="n_box">
        <Nflexbox/>
    </div>
</template>
<script>
import Nflexbox from './common/Flexbox.vue'
    export default {
        name:'NGroupLayout',
         components: {
            Nflexbox
        }
    }
</script>

<style lang="stylus">
div.n_box
    padding 10px
    box-sizing border-box
    overflow hidden
</style>