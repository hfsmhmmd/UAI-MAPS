<template>
  <div id="app">
    <ExploreView/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import ExploreView from './views/ExploreView.vue'
export default {
  name: 'App',
  components: {
    ExploreView
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
