<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
   <section class="text-center flex flex-col items-center justify-center h-96">
      <i class="pi pi-exclamation-triangle text-yellow-500 text-7xl mb-5"></i>
      <h1 class="text-6xl font-bold mb-4">404 Page Not Found</h1>
      <p class="text-xl mb-5">This page does not exists</p>
      <RouterLink to="/" class="text-white bg-green-700 p-2 mt-4 rounded-md">
         Go Back
      </RouterLink>
   </section>
</template>
