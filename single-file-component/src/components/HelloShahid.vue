<script setup>
import HelloAmir from './HelloAmir.vue'
const m='this is child componenet HelloShahid Vue'
</script>

<template>
  <div>
    <h2>it is helloshahid component its child is hello-amir and paraent is app.vue</h2>
    <h1>{{ m }}</h1>
  <hello-amir />
  </div>
</template>

<style scoped>
div{
  height: 40vh;
  background-color: cadetblue;
}
h1{
  background-color: #0f0;
}
</style>