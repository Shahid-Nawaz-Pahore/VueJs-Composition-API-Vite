<script setup>
const x =+prompt('Enter Number 1:');
const y=+prompt('enter number 2:');

function add(){
  return x+y
}
</script>
<template>
  
<div>
  <h1>{{ x }}</h1> 
  <h1>{{ y }}</h1>
  <h1>{{add()%2==0? `${x}  and ${y}equal to: ${x+y} is even Number`:`${x} and ${y} is not equal to : ${x+y} is odd number` }}</h1>
</div>
</template>