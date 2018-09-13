<template>
    <div class="n_box">
        <Nflexbox :listData="listData">
        </Nflexbox>
    </div>
</template>
<script>
import iconpath from'../assets/images/1.png'
import Nflexbox from './common/Flexbox.vue'
    export default {
        name:'NGroupLayout',
         components: {
            Nflexbox
        },
        data(){
            return{
                listData:[{
                    id:'0001',
                    title:'这是商品名称',
                    desc:'这是一段描述性文字',
                    icon: iconpath
                },
                {
                    id:'0002',
                    title:'这是商品名称',
                    desc:'这是一段描述性文字',
                    icon: iconpath
                }]
            }
        }
    }
</script>

<style lang="stylus">
div.n_box
    padding 10px
    box-sizing border-box
    overflow hidden
</style>