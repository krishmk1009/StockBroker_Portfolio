<template>
   <div class="max-w-7xl mx-auto my-20">

    <div>
        <h2 class="text-4xl font-bold text-center mb-8 text-gray-600">Our Services</h2>
    </div>

    <div class="flex justify-evenly">
        <div class="w-1/4" v-for="(section , index) in ServiceSectionContent.services"
        :key="index"
        >
            <div>
                <img :src="section.ServiceImage"
                class="w-48 h-48 rounded-lg mx-auto"
                :alt="section.ServiceImageAlt"
                />
            </div>
            <div class="text-center">
                <h3 class="text-xl font-bold mb-2 my-2">{{section.ServiceHeading}}</h3>
                <p class="text-gray-600 mb-4 mx-4">

                   {{ section.ServiceSubHeading }}
                </p>
                <button class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full">
                    {{ section.ServiceButton }}
                </button>
            </div>
        </div>

        
       
    </div>

   </div>
  </template>
  
  <script setup lang="ts">
  import Card from './Card.vue';
  import { ServiceSectionContent } from '../constant';
  </script>
  
  <style>
  body {
    margin: 0;
    font-family: Arial, sans-serif;
  }
  </style>
  