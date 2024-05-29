<template>
    <div class="my-10 max-w-7xl mx-auto">
      <div class="flex justify-center">
        <img
          :src="AboutSectionContent.AboutUsImage"
          class="w-full  object-cover h-80"
        />
      </div>
      <div>
        <h2 class="text-4xl font-bold text-center mb-8 my-4">{{AboutSectionContent.AboutUsHeading}}</h2>
        <p class="text-center text-gray-600 w-1/2 mx-auto">
          {{AboutSectionContent.AboutUsDescription}}
        </p>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import { AboutSectionContent } from '../constant';
  </script>
  