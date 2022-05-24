<template>
  <div id="app">
        <!-- <ExploreView/> -->
      <nav>
     
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> | -->
      <router-link to ="/explore"> Explore Lantai</router-link> |
      <router-link to ="/mappage"> Halaman Peta</router-link>
    </nav>
    <router-view/>
 
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import ExploreView from './views/ExploreView.vue'
export default {
  name: 'App',
  components: {
    // ExploreView
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
