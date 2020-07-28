<template>
  <div id="app">
    <!-- <MParent></MParent> -->
    this is app
    <br />
    <router-link to="/home">go home</router-link>
    <router-view></router-view>
    <button @click="toHome"></button>
  </div>
</template>

<script>
// import MParent from './views/Parent'

export default {
  // components: { MParent },
  methods: {
    toHome () {
      this.$router.push({ path: '/home', query: { name: '张三}' } })
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
