<script setup>
import { Fragment } from 'vue';
import HelloShahid from './components/HelloShahid.vue'
import HelloZahid from './components/HelloZahid.vue'
const msg='this is parent componenet app Vue'
</script>

<template>
<div id="app">
  <h2>App vue it has two child component hellozahid and helloshahid</h2>
  <div class="header">
    <h1>{{ msg }}</h1>
  </div>
  <div class="main">
    <hello-zahid/>
  </div>
  <div class="footer">
    <HelloShahid/> 
  </div>
</div>
</template>

<style scoped>
#app{
  width: 100%;
  height: 100vh;
  background-color: rgb(11, 44, 44);
}
h1{
  background-color: #f00;
}
</style>