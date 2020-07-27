<template>
  <div id="app">
    <MParent></MParent>
  </div>
</template>

<script>
import MParent from './views/Parent'

export default {
  components: { MParent },
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
