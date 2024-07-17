<script setup>
import { RouterLink } from 'vue-router'
import JobData from '@/jobs.json'
import JobListing from '@/components/JobListing.vue'
import { ref, defineProps } from 'vue'
const jobs = ref(JobData)

defineProps({
   limit: {
      type: Number
   },
   showButton: {
      type: Boolean,
      default: false,
   }
})
</script>

<template>
   <section class="bg-blue-50 px-4 py-10">
      <div class="container-xl lg:container m-auto">
         <h2 class="text-3xl font-bold text-green-600 mb-6 text-center">
            Browse Jobs
         </h2>
         <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <JobListing v-for="job in jobs.slice(0, limit || jobs.length)" :key="job.id" :job="job" />
         </div>
      </div>
   </section>

   <section v-if="showButton" class="m-auto max-w-lg py-10 px-6 text-center">
      <RouterLink class="text-center block bg-black rounded-lg py-4 px-6 text-white hover:bg-gray-700" to="/jobs">
         View All Jobs
      </RouterLink>
   </section>
</template>
