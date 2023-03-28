<script setup>
import {ref} from 'vue'
const isActive=ref(true)
const Num=ref(1)
const ch=ref('J')
</script>
<template>
  <div>
    <h1 v-if="true">v-if is true</h1>
  <h1 v-if="isActive">v-f isActive</h1>
  <!-- //v-f and v-else -->
  <h1 v-if="Num%2===0">number {{ Num }} is even</h1>
  <h1 v-else>number {{ Num }} is not odd</h1>
  <!-- //v-if v-else-if v-else  -->
  <h1 v-if="ch==='A'">A</h1>
  <h1 v-else-if="ch==='B'">B</h1>
  <h1 v-else-if="ch==='C'">C</h1>
  <h1 v-else-if="ch==='D'">D</h1>
  <h1 v-else-if="ch==='E'">E</h1>
  <h1 v-else-if="ch==='F'">F</h1>
  <h1 v-else>NOT A/B/C/D/E/F</h1>
  <!-- template if elase -->
  <template v-if="false">
<h1>template v-if true</h1>
  </template>
  <template v-else>
  <h1>template else</h1>
  </template>
  <h1 v-show="true">v-show true</h1>



  </div>

</template>