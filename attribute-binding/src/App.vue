<script setup>
const id="header"
const clas='header'
const type = 'text'
const name='input'
const value='value'
const placeholder='enter input'
const multipleAttributes= {
       id:"header",
        clas:'header',
        type : 'text',
        name:'input',
        value:'value',
        placeholder:'enter input'

}
const href="https://www.youtube.com/"
const url="href"
</script>

<template>
  <div class="">
    <h1>binding attributes</h1>
    <input :id="id" :name="name" :class="clas" :type="type" :value="value" :placeholder="placeholder">
     <h1>binding multiple attributes dynimically </h1>
     <input :="multipleAttributes"><br>
     <a :[url]="href">youtube</a>
  </div>
  
</template>