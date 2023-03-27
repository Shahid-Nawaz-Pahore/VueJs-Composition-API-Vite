<script setup>
import {ref} from 'vue'
let fName=ref('shahid')
let lName=ref('nawaz')
let age=ref(23)


function display(){
  return  `my name is ${fName.value} ${lName.value} and my age is ${age.value}`
  
}
setTimeout(()=>{
  console.log('change the values')
  fName.value='zahid'
  lName.value='amir'
  age.value=30
},2000)
</script>

<template>
  <div>
    <h1>who i am ?</h1><hr><hr>
  <h1>{{ display() }}</h1>
  </div>
</template>