<template>
    <div class="n_form_group">
        <NInput type="tel"  placeholder="请输入手机号"/>
        <NInput type="password"  placeholder="请输入密码"/>
    </div>
</template>
<script>
import NInput from './common/Input.vue'
    export default {
        name:'login',
         components: {
            NInput
        }
    }
</script>

<style lang="stylus">
div.n_form_group
    .n_input
        margin-bottom 10px

</style>