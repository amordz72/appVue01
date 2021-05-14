<template>
  <h1>{{ msg }}</h1>
 <h1  >{{title}}</h1>
  <p>
 <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>
  <h3>{{ state.count }}</h3>
 <button @click="state.count++"> ++</button>
  <button @click="state.count--"> - - </button>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String,    title: String,  
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
h3{
 
}


</style>
