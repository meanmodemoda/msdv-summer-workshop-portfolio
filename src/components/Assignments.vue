<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <br>
    <br>
    <p>A 6 week training outcome to get started with HTML, CSS and JavaScript.<br>I've learned to build a responsive webpage, JavaScript essentials and JavaScript key frameworks.</p>
    <div class="portfolio">
    <ul>
      <li><div class="container"><a href="https:///muonius.github.io/msdv-summer-workshop-about-me/" target="_blank" rel="noopener">
        <img alt="Assignment 1" src="./Assignment_1_Square.jpg"> 
        <div class="overlay"><div class="text"><h3>Assignment 1</h3>
          <p>Create a responsive "About Me" page.</p></div>
        </div></a></div></li>
        
      <li><div class="container"><a href="https://muonius.github.io/msdv-summer-workshop-javascript-functions" target="_blank" rel="noopener"> 
      <img alt="Assignment 2" src="./Assignment_2_Square.jpg">
      <div class="overlay"><div class="text"><h3>Assignment 2</h3>
        <p>Practice JavaScript functions and console log results.</p></div>
      </div></a></div></li>
      
      <li><div class="container"><a href="https://muonius.github.io/msdv-summer-workshop-javascript-data-rendering/" target="_blank" rel="noopener">   
       <img alt="Assignment 3" src="./Assignment_3_Square.jpg">
      <div class="overlay"><div class="text"><h3>Assignment 3</h3>
        <p>Render data using JavaScript in increments of 5 and add pagination.</p></div>
      </div></a></div></li>

      <li><div class="container"><a href="https://muonius.github.io/msdv-summer-workshop-d3-chart/" target="_blank" rel="noopener">  
      <img alt="Assignment 4.1" src="./Assignment_4_1_Square.jpg">
      <div class="overlay"><div class="text"><h3>Assignment 4.1</h3>
        <p>Plot a bar chart using d3.js.</p></div>
      </div></a></div></li>
      
      <li><div class="container"><a href="https://muonius.github.io/msdv-summer-workshop-p5-bar-chart/" target="_blank" rel="noopener">  
      <img alt="Assignment 4.2" src="./Assignment_4_2_Square.jpg">
      <div class="overlay"><div class="text"><h3>Assignment 4.2</h3>
        <p>Plot a bar chart using p5.js.</p></div>
      </div></a></div></li>
      
        <li><div class="container"><a href="https://muonius.github.io/msdv-summer-workshop-vue-render-and-filter-data/" target="_blank" rel="noopener">  
     <img alt="Assignment 5" src="./Assignment_5_Square.jpg">
      <div class="overlay"><div class="text"><h3>Assignment 5</h3>
        <p>Use Vue.js to render data and add a text based filter.</p></div>
      </div></a></div></li>
      
      </ul>
    </div>
  </div>
   
</template>

<script>
export default {
  name: 'Assignments',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h3 {
  margin: 40px 0 0;
}

p {
  font-size: 16px;
}

.portfolio ul {
  display: inline-block;
  list-style-type: none;
  padding: 0;
}


.portfolio li {
  display: inline-block;
  margin: 20px 20px;
  /*position: relative;*/
}

a {
  color: #42b983;
}

.container {
  position: relative;
  border: 0.1rem solid black;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: white;
}

img {
  display: block;
  width: 300px;
  height: 100%;
}

.text {
  color: black;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;

}

img:hover {
  opacity: 0.3;
}

li:hover .text {
  opacity: 1;
}

.container:hover .overlay {
  opacity: 1;
}


</style>
