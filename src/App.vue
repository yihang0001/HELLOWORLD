<template>
  <div id="app" >
   <div v-show="isShow"><br/>
    <h2>永远相信美好的事情即将发生</h2><br/>
     <h2>祝发财!</h2><br/>
     <h2>---来自 蔡</h2>
     </div>
   <button v-on:click="showorhide()">你好</button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  data:{
   isShow: true
  },
  components: {
    HelloWorld
  },
  methods:{
  showorhide:function(){
  this.isShow = !this.isShow;
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
