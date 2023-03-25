<script setup>
import { reactive} from 'vue'
let number = reactive({
  a:22,
  b:39
})
setTimeout(()=>{
  console.log('timeout function is called')
  console.log("number" ,number)
  number.a=98,
  number.b=878,
  
  console.log(`value of ${number.a} and ${number.b}`)
},2000)
</script>


<template>
 <h1>{{ number.a+number.b }}</h1>
</template>