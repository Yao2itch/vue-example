<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <!-- <vue-file-toolbar-menu :content="my_menu"/> -->
</template>

<script>
// import VueFileToolbarMenu from 'vue-file-toolbar-menu'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    // VueFileToolbarMenu,
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
