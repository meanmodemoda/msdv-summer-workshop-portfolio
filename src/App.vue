<template>
  <div id="app">
   <a href="https://muons.com/msdv-summer-workshop-about-me/" target="_blank" rel="noopener"><img alt="Vue logo" src="./assets/logo.png"></a> 
    <span></span>
    <h1>MS Data Visualization Summer Workshop 2021</h1>
    <Assignments msg="Assignment Portfolio"/>
  </div>
</template>

<script>
import Assignments from './components/Assignments.vue'

export default {
  name: 'App',
  components: {
    Assignments
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

img {
  height: 150px;
}
</style>
