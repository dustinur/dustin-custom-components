<template>
  <div id="app">
    <my-header></my-header>
    <server-details></server-details>
    <servers></servers>
    <my-footer></my-footer>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import ServerDetails from './components/ServerDetails.vue'
import Servers from './components/Servers.vue'

export default {
  name: 'app',
  components: {
    'hello-world' : HelloWorld,
    'my-header' : Header,
    'server-details' : ServerDetails,
    'servers' : Servers,
    'my-footer' : Footer
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding: 20px;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
