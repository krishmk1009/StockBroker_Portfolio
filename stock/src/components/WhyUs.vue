<template>
    <div class="max-w-7xl mx-auto my-20">
 
     <div>
         <h2 class="text-4xl font-bold text-center mb-8">Why Us</h2>
     </div>
 
     <div class="flex justify-evenly">
         <div v-for="(section , index) in WhyUSSectionContent.descriptions"
         :key="index"
         class="w-1/3"
         >
             <div class="">
                 <img :src="section.imageSrc"
                    class="w-24 h-24 rounded-lg mx-auto"
                 />
             </div>
             <div class="text-center">
                 <p class="text-gray-600 my-4 w-3/4 mx-auto"> {{ section.description }}
                </p>
             </div>
         </div>
    
     </div>
 
    </div>
   </template>
   
   <script setup lang="ts">
   import { WhyUSSectionContent } from '../constant';
   </script>
   
   <style>
   body {
     margin: 0;
     font-family: Arial, sans-serif;
   }
   </style>
   