<script setup lang="ts">
import { reactive } from 'vue';
 console.log(1234567);
 const state = reactive({
  count: 7
 })
 const onAdd = ()=>{
  state.count ++ 
 }
</script>
<template>
  <div class="about">
    <h1>This is an about page {{ state.count }}</h1>
    <button @click="onAdd">+</button>
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
