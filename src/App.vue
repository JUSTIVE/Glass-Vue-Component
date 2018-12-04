<template>
  <div id="app">
    <glassmaterial msg=""/>
  </div>
</template>

<script>
import glassmaterial from './components/glassmaterial.vue'

export default {
  name: 'app',
  components: {
    glassmaterial
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
