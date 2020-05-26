<template>
  <div id="app">
   <landing></landing>
  </div>
</template>

<script>
import Landing from './components/Landing.vue'


export default {
  name: 'App',
  components: {
    Landing
  }
}
</script>

<style>
@import "./assets/css/core.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
