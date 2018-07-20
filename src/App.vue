<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <!-- <ul>
      <li><a href="https://vuejs.org" target="_blank">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank">Twitter</a></li>
    </ul>
    <h2>Ecosystem</h2> -->
    <!-- <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul> -->
    <br>
    <el-button type="success">我的按钮</el-button>
    <el-button type="primary" icon="el-icon-search">搜索</el-button>
    <el-row>
      <el-col :span="24"><div class="grid-content bg-purple-dark">第一行</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="8"><div class="grid">第二行第1列</div></el-col>
      <el-col :span="8"><div class="grid">第二行第2列</div></el-col>
      <el-col :span="8"><div class="grid">第二行第2列</div></el-col>
    </el-row>
    <Datepicker></Datepicker>
  </div>
</template>

<script>
import Datepicker from './componets/Datepicker.vue'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
    }
  },
  components:{
    Datepicker
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.grid {
  border: 1px solid  #333;
  font-size: 12px
}
</style>
