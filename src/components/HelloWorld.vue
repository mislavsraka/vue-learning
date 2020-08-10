<template>
  <div class="container">
    <div>{{ msg }}</div>
    <div v-html="text" class="square" v-bind:class="size" v-bind:style="{backgroundColor:color}">
  </div>
  </div>
</template>

<script>
export default {
   name: 'Square',
   props: {
    color: String,
    size: String,
    text: String
  }
}
</script>

<style scoped>
.square {
    background-color: blue;
    color: #fff;
    margin: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
.small {
  height: 50px;
  width: 50px;
  background-color: yellow;
}
.medium {
  height: 150px;
  width: 150px;
  background-color: green;
}
.large {
  height: 250px;
  width: 250px;
  background-color: red;
}
</style>
