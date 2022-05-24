<template>
  <div id="app">

       
      <nav>
      <router-link to ="/explore" class="rout"> Explore Lantai  </router-link>   
      <!-- <router-link to ="/mappage" class="rout">   Halaman Peta</router-link> -->
    </nav>
    <router-view/>
  </div>
</template>
<script>

export default {
  name: 'App',
  components: {
    // ExploreView
  }
}
</script>

<style>
html, body{
  height: 100%;
  
}


#app {
  display: flex;
   flex-direction: column;
  align-self: flex-end;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color:#0E47A1;
  height: 100%;
    
}
nav{
  display: flex;
  height: 30px;
  color: #0E47A1;
  justify-content: center;
  background-color: white;
  bottom:5px;
}
.rout{
  color: #0E47A1;
}
</style>
