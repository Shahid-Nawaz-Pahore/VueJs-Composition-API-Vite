<script setup>
import { ref, reactive } from 'vue'
const cl = ref('red')
const bg = ref('green')
const obj=reactive({
  color:'blue',
  backgroundColor:'black'
})
const obj1=reactive({
  color:'blue',
  backgroundColor:'green'
})
const obj2=reactive({
  fontSize:'100px',
})
</script>
<template>
  <div>
    <!-- simple -->
    <h1 style="color: rebeccapurple;background-color: bisque;">simple style</h1>
    <!-- binding style -->
    <h1 :style="{color:'red',backgroundColor:'yellow'}"> bind style </h1>
    <!-- style using ref -->
    <h1 :style="{color:cl,backgroundColor:bg}"> bind style by ref </h1>
    <!-- style using reactive -->
    <h1 :style="obj"> bind style by reactive </h1>
    <!-- binding style by array of objects  -->
    <h1 :style="[obj1,obj2]"> bind style by array of object </h1>
  </div>
</template>