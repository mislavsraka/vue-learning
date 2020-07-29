<template>
  <div id="app">
    <HelloWorld msg="Klasa square" />
    <HelloWorld msg="Klasa small" size="small"/>
    <HelloWorld msg="Klasa medium" size="medium"/>
    <HelloWorld msg="Klasa large" size="large"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
}
</style>
