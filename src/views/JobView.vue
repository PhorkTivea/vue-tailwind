<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
   <section class="bg-green-50">
      <div class="container m-auto py-10 px-6">
         <div class="grid grid-cols-1 w-full gap-6 md:grid-cols-70/30">
            <main>
               <div class="bg-white p-6 rounded-lg text-center shadow-md md:text-left">
                  <div class="text-gray-500 mb-4">Full-Name</div>
                  <h1 class="text-3xl font-bold mb-4">Senoir Vue Developer</h1>
                  <div class="text-gray-500 mb-4 flex align-middle justify-center md:justify-start">
                     <i class="pi pi-map-marker text-xl text-orange-700 mr-2"></i>
                     <p class="text-orange-700">Phnom Penh</p>
                  </div>

                  <div class="bg-white p-6 rounded-lg shadow-md mt-6">
                     <h3 class="text-green-800 text-lg font-bold mb-6">Job description</h3>
                     <p class="mb-4">Hello welcome on board anny if you have any question feel free to ask me!</p>
                     <h3 class="text-green-800 text-lg font-bold mb-2">Salary</h3>
                     <p class="mb-4">70k / year</p>
                  </div>
               </div>
            </main>

            <aside>
               <div class="bg-white p-6 rounded-lg shadow-md">
                  <h3 class="text-xl font-bold mb-6">Company Info</h3>
                  <h2 class="text-2xl">Khits</h2>
                  <p class="my-2">Hello welcome on board anny if you have any question feel free to ask me!</p>
                  <hr class="my-4">
                  <h3 class="text-xl">Contact Email: </h3>
                  <p class="my-2 bg-green-100 p-2 font-bold">Khits@phnompenhgmail.com</p>
                  <h3 class="text-xl"> Phone: </h3>
                  <p class="my-2 bg-green-100 p-2 font-bold">0987654321</p>
               </div>

               <div class="bg-white p-6 rounded-lg mt-6 shadow-md">
                  <h3 class="text-xl font-bold mb-6">Manage Job</h3>
                  <RouterLink to="/"
                     class="bg-green-500 text-white hover:bg-green-600 font-bold py-2 px-4 rounded-full w-full focus:outline-none focus:shadow-outline mt-4 block text-center">
                     Edit
                  </RouterLink>
                  <button
                     class="bg-red-500 hover:bg-red-600 text-white font-bold py-2 px-4 rounded-full w-full focus:outline-none focus:shadow-outline mt-4 block">
                     Delete Job
                  </button>
               </div>
            </aside>
         </div>
      </div>
   </section>
</template>
