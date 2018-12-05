<template>
  <div id="app">
    <glassmaterial msg="" size="300px" depth="12px"/>
  </div>
</template>

<script>
import glassmaterial from './components/glassmaterial.vue'
// import glassmaterial1 from './components/glassmaterial.1.vue'

export default {
  name: 'app',
  components: {
    glassmaterial
    // glassmaterial1
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
