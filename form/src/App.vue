<script setup>
import {reactive} from 'vue'
const formData=reactive({
  name:'shahid',
  email:'shahid@gmail.com',
  password:'password',
  message:'message',
  hobies:[],
  gender:'',
  jobpost:'',
  selectLocation:[],
  fee:'',
})
 const states=reactive([
  {text:'panjab',value:'panjab'},
  {text:'lahore',value:'lahore'},
  {text:'sindh',value:'sindh'},
    {text:'islamabad',value:'islamabad'},
    ]
 )
function formHandle(){
  console.log(formData)
}
</script>

<template>
  
  <form @submit.prevent="formHandle">
    <pre>{{ formData}}</pre>
  <div>
    <label for="name">Name:</label>
    <input type="text" id="name" v-model.trim="formData.name">
  </div>
  <div>
    <label for="email">Email:</label>
    <input type="email" id="email" v-model="formData.email">
  </div>
  <div>
    <label for="password">password:</label>
    <input type="password" id="password" v-model="formData.password">
  </div>
  <div>
    <label for="message">message:</label>
    <textarea  id="message" v-model="formData.message"></textarea>
  </div>
  <div>
    <span>Hobbies:</span>
    <label for="reading">reading</label>
    <input type="checkbox" id="reading" value="reading"  v-model="formData.hobies">
    <label for="cooking">cooking</label>
    <input type="checkbox" id="cooking" value="cooking"  v-model="formData.hobies">
    <label for="listing">listing</label>
    <input type="checkbox" id="listing" value="listing"  v-model="formData.hobies">
    <label for="watching">watching</label>
    <input type="checkbox" id="watching" value="watching"  v-model="formData.hobies">
  </div>
  <div>
    <span>gender:</span>
    <label for="male">Male</label>
    <input type="radio" id="male" value="male" v-model="formData.gender">
    <label for="female">female</label>
    <input type="radio" id="female" value="female" v-model="formData.gender">
    <label for="other">other</label>
    <input type="radio" id="other" value="other" v-model="formData.gender">
  </div>
  <div>
    <span>Job Post</span>
    <select v-model="formData.jobpost">
    <option disabled  value=""> Select job post</option>
    <option  > laravel developer</option>
    <option  > Vue developer</option>
    <option  > angular developer</option>
    </select>
  </div>
  <div>
    <span>Select Job Lacation</span>
    <select v-model="formData.selectLocation">
    <option v-for="(state,index) in states" :key="index" :value="state.value">{{ state.text }}</option>
    </select>
  </div>
  <div>
    <label for="fees">Fees</label>
    <input type="text" id="fees" v-model.number="formData.fee">
  </div>
  <button type="submit">Submit</button>
</form>
</template>