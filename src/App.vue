<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Toolbar from './components/Toolbar.vue'
import GithubUserInfo from './components/GithubUserInfo.vue'
</script>

<template>
   <Toolbar/>
  
   <div class="container-fluid">
     <div class="row">
       <div class="col-md-12">
         <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores facere repellendus alias vero assumenda? Sunt distinctio quis alias culpa voluptatum nemo non nisi ad minus, dolor optio, fugit unde eius!</p>
         <GithubUserInfo />
       </div>
     </div>
   </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
