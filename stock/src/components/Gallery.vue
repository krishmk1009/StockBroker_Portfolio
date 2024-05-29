<template>
    <div class="max-w-7xl  m-auto">
        <h2 class="text-4xl font-bold text-center mb-8">Gallery</h2>

  
    <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
      <div v-for="(image, index) in GallerySectionContent.images" :key="index">
        <img class="h-auto max-w-full rounded-lg" :src="image.src" :alt="image.alt" />
      </div>
    </div>
</div>
  </template>
  
  <script setup lang="ts">
  import { GallerySectionContent } from '../constant';
  </script>
  