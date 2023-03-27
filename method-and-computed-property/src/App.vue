<script setup>
import {ref , computed} from 'vue'
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

//computed property
let x=ref(10)
let y=ref(30)
const sum=computed(()=>{
  return x.value+y.value
})
setTimeout(()=>{
  x.value=200
  y.value=87338
},2000)

</script>

<template>
  <div>
    <h1>Method in vuejs</h1>
      <h1>{{ display() }}</h1>
      <hr><hr>
      <h1>computed property in vuejs</h1>
      <h1>{{ sum }}</h1>
      <p>computed property is fast then method when states are not changing  becase it create cashe </p>
  </div>
</template>