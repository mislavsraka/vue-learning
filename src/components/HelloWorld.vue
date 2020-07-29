<template>
  <div class="container">
    <div>{{ msg }}</div>
    <div class="square" :class="size" />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    size: String
  },

}
</script>

<style scoped>
.square {
  height: 200px;
  width: 200px;
  background-color: blue;
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
