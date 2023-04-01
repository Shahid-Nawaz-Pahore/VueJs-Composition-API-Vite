<script setup> 
import {ref} from 'vue'
//array
//const students=ref(['amir','kamran','zahid','shahid'])

// object in array
// const students=ref([
//   {name:'shahid nawaz',roll:10,age:23},
//   {name:'zahid nawaz',roll:11,age:20},
//   {name:'amir nawaz',roll:18,age:25},
//   {name:'kamran nawaz',roll:19,age:13}
// ])

const arr=ref([
  [1,2,3,4],
  [a,b,c,d]
])
</script>

<template>
  <div>
    <!-- array -->
    <!-- <h1 v-for="(student,index) in students" :key="index">{{ index }} {{ student }}</h1> -->
    <!-- objects in array -->
  <!-- <h1 v-for="(student, index) in students"  :key="index">{{ index }} {{ `Name:${student.name} Roll#:${student.roll} age:${student.age} ` }}</h1> -->


  </div>
</template>