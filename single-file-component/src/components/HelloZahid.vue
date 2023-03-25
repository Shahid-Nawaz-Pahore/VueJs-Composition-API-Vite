<script setup>
import HelloKamran from './HelloKamran.vue'
const m='this is child componenet HelloZahid Vue'
</script>

<template>
  <div>
    <h2>hello zahid component its paranet is app.vue and child is hellokamran</h2>
    <h1>{{ m }}</h1>
    <hello-kamran/>
  </div>
</template>

<style scoped>
div{
  background-color: blueviolet;
  height: 30vh;
}
h1{
  background-color: #9f0;
}
</style>