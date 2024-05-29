<template>
    <div class="card bg-white shadow-lg rounded-lg p-6 text-center">
      <img class="w-32 h-32 rounded-lg mx-auto mb-4" :src="image" alt="Card Image" />
      <h3 class="text-xl font-bold mb-2">{{ heading }}</h3>
      <p class="text-gray-600 mb-4">{{ subheading }}</p>
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        {{ buttonText }}
      </button>
    </div>
  </template>
  
  <script setup lang="ts">
  import { defineProps } from 'vue';
  
  interface Props {
    image: string;
    heading: string;
    subheading: string;
    buttonText: string;
  }
  
  const props = defineProps<Props>();
  </script>
  
  <style scoped>
  .card {
    max-width: 300px;
    margin: auto;
  }
  </style>
  