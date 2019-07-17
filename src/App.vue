
<template>
  <div id="app">
    <div id="nav">
      <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand right v-on:click="goto('home')">AMP</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item right v-on:click="goto('about')">About</b-nav-item>
            <b-nav-item right v-on:click="gotop('projects')">Projects</b-nav-item>
          <b-nav-item right v-on:click="gotoc('contact')">Contact Me</b-nav-item>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
        
        </b-collapse>
      </b-navbar>
    </div>
    <router-view/>
  </div>
</template>
<script>
// @ is an alias to /src
import $ from "jquery";
export default {

  name: 'App',
  
  data() {
      return {
        
      }
    },
    methods: {
      goto(page){
        $('html, body').animate({
            scrollTop: $("#about").offset().top
        }, 1000);
      }
   
      , gotoh(page){
        $('html, body').animate({
            scrollTop: $("#home").offset().top
        }, 1000);
      }
      
      , gotop(page){
        $('html, body').animate({
            scrollTop: $("#projects").offset().top
        }, 1000);
      }
      
      , gotoc(page){
        $('html, body').animate({
            scrollTop: $("#contact").offset().top
        }, 1000);
      }
      
  }
}

</script>
<style>
body{
  margin: 0px;
  color: white !important;
  background-color: black !important;
}

a:hover{
  cursor: pointer;
}

#app {
  font-family: 'Source Sans Pro', sans-serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  
}
#nav {
  padding: 30px;
  position: fixed;
  z-index: 1;
  height: 85px;
  width: 100vw;
  
  margin: 0px;
  padding: 0px;
}

.navbar{
 height: 85px;
}

#app .bg-info {
    background-color: black !important;
}

#nav a {
  font-weight: bold;
  
  display:inline-block;
  margin: 0px;
  padding: 25px 10px;
  
}

.navbar-nav li{
  z-index: 300 !important;
  background-color: rgba(0, 0, 0, 0.842);
}


.vertcenter{
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}
</style>

