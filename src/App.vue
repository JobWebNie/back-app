<template>
  <div id="app">
    <HelloWorld msg="移动端 常用组件"/>
    <Login />
    <Layout />
    <Tabbar v-model="select" v-on:tapTabItem="addLister">
        <TabItem id='tab1'>
            <img slot="icon" src="./assets/images/1.png" alt="商品图片">
            外卖
        </TabItem>
         <TabItem id='tab2'>
            <img slot="icon" src="./assets/images/1.png" alt="商品图片">
            外卖
        </TabItem>
        <TabItem id='tab3'>
            <img slot="icon" src="./assets/images/1.png" alt="商品图片">
            外卖
        </TabItem>
        <TabItem id='tab4'>
            <img slot="icon" src="./assets/images/1.png" alt="商品图片">
            外卖
        </TabItem>
    </Tabbar>
    <Register />
    <Toast />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Login from './components/Login.vue'
import Layout from './components/Layout.vue'
import Tabbar from './components/common/Tabbar/index.vue'
import TabItem from './components/common/Tabbar/TabItem.vue'
import Register from './components/common/Register.vue'
import Toast from './components/common/Toast.vue'
export default {
  name: 'app',
  components: {
    HelloWorld,
    Login,
    Layout,
    Tabbar,
    TabItem,
    Toast,
    Register
  },
  data(){
    return{
      select:"tab1"
    }
  },
  methods:{
    addLister(id){
      // console.log(id)
      this.select = id
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
