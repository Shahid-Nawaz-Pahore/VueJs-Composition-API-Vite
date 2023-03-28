<script setup> 
import {ref} from 'vue'
const students=ref(['amir','kamran','zahid','shahid'])
</script>

<template>
  <div>
    <h1 v-for="(student,index) in students" :key="index">{{ index }} {{ student }}</h1>
  </div>
</template>