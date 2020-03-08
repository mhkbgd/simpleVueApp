<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/black.gif">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Test msg="This is test"/>
    <Contact />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Test from './components/test.vue'
import Contact from './components/contact.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Test,
    Contact
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
