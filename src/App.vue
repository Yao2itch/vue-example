<template>
  <vue-file-toolbar-menu :content="my_menu"/>
</template>

<script>
import VueFileToolbarMenu from 'vue-file-toolbar-menu'
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    VueFileToolbarMenu,
    // HelloWorld
  },
   computed: {
    classObject: function () {
      return {
        base: true,
        active: true,
        'text-danger': "",
      }
    },
    my_menu () {
      return [
        { text: "My Menu", menu: [
          { text: "Item 1", click: () => alert("Action 1") },
          { text: "Item 2", click: () => alert("Action 2") }
        ] }, {
          text: "My Button",
          active: this.happy,
          icon: this.happy ? "sentiment_very_satisfied" : "sentiment_satisfied",
          click: () => { this.happy = !this.happy }
        }
      ]
    }
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
