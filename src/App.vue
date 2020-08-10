<template>
  <div id="app">
<!--     <HelloWorld msg="Klasa square" />
    <HelloWorld msg="Klasa small" size="small"/>
    <HelloWorld msg="Klasa medium" size="medium"/>
    <HelloWorld text="This is a square" size="large" color="#000"/> -->
    <HelloWorld
      v-for="data in myJson"
      v-bind:key="data.text"
      v-bind:text="data.text"
      v-bind:size="data.size"
      v-bind:color="data.color"
    />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import json from './json/data.json'

export default {
  name: 'App',
  data(){
    return{
      myJson: json
    }
  },
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
