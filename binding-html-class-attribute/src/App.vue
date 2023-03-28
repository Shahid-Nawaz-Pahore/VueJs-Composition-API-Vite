<script setup>
import {ref , reactive , computed} from 'vue'
const isActive = ref(true)
const isImportant=ref(true)
const obj=reactive({
  active:true,
  'f-bold':true,
  fontSize:true
})
</script>

<template>
  <div>
    <h1 class="text-red f-bolder">hello</h1>
    <h1 v-bind:class="{'active':isActive ,'f-bold':isImportant}">assign class using ref</h1>
    <h1 v-bind:class="obj">assign class using reactive object</h1>
    <h1 :class="isActive?'active':'notActive'">kjd</h1>
</div>
</template>