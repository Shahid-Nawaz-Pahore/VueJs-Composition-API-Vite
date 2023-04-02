<script setup>
const fullName = defineProps(['firstName', 'lastName'])
</script>

<template>
  <div class="about">

    <pre>
      <h1>{{ fullName }}</h1>
      <h1>{{ firstName }}</h1>
      <h1>{{ lastName }}</h1>
    </pre>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
