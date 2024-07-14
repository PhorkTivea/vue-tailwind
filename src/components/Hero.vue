<script setup>
import { defineProps } from 'vue'
defineProps({
   title: {
      type: String,
      default: 'Become A Vue Dev'
   },
   subtitle: {
      type: String,
      default: 'Find the vue job that fits your skills and needs'
   }
})
</script>

<template>
   <section class="bg-green-700 py-20 mb-4">
      <div class="max-w-7xl mx-auto">
         <div class="text-center">
            <h1 class="text-white text-4xl font-extrabold sm:text-5xl md:text-6xl">{{ title }}</h1>
            <p class="my-4 text-xl text-white">
               {{ subtitle }}
            </p>
         </div>
      </div>
   </section>
</template>
