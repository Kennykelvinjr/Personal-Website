<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
</script>

<template>
  <NavBar />
  <RouterView v-slot="{ Component }">
    <Transition name="fade" mode="out-in"> <component :is="Component" /> 
    </Transition>
  </RouterView>  
</template>

<style scoped>
</style>
