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
html, body, #app #app>div{
  height: 100%;
}


#app {
  display: flex;
   flex-direction: column;
 
  
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #0E47A1;
  /* height: 100%; */
  border: 5px solid greenyellow;
}

</style>
