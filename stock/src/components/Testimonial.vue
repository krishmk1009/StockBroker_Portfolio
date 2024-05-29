<template>
    <div class="min-w-screen flex items-center justify-center py-5">
      <div class="w-full bg-white border-t border-b border-gray-200 px-5 py-16 md:py-24 text-gray-800">
        <div class="w-full max-w-6xl mx-auto">
          <div class="text-center max-w-xl mx-auto">
            <h1 class="text-6xl md:text-5xl font-bold mb-5 text-gray-600">{{ TestimonialSectionContent.title }}</h1>
            <h3 class="text-xl mb-5 font-light">{{ TestimonialSectionContent.subtitle }}</h3>
            <div class="text-center mb-10">
              <span class="inline-block w-1 h-1 rounded-full bg-blue-500 ml-1"></span>
              <span class="inline-block w-3 h-1 rounded-full bg-blue-500 ml-1"></span>
              <span class="inline-block w-40 h-1 rounded-full bg-blue-500"></span>
              <span class="inline-block w-3 h-1 rounded-full bg-blue-500 ml-1"></span>
              <span class="inline-block w-1 h-1 rounded-full bg-blue-500 ml-1"></span>
            </div>
          </div>
          <div class="-mx-3 md:flex items-start">
            <div v-for="(testimonialGroup, index) in TestimonialSectionContent.testimonialGroups" :key="index" class="px-3 md:w-1/3">
              <div v-for="testimonial in testimonialGroup" :key="testimonial.id" class="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                <div class="w-full flex mb-4 items-center">
                  <div class="overflow-hidden rounded-full w-10 h-10 bg-gray-50 border border-gray-200">
                    <img :src="testimonial.imgSrc" :alt="testimonial.name">
                  </div>
                  <div class="flex-grow pl-3">
                    <h6 class="font-bold text-sm uppercase text-gray-600">{{ testimonial.name }}</h6>
                  </div>
                </div>
                <div class="w-full">
                  <p class="text-sm leading-tight">
                    <span class="text-lg leading-none italic font-bold text-gray-400 mr-1">"</span>
                    {{ testimonial.message }}
                    <span class="text-lg leading-none italic font-bold text-gray-400 ml-1">"</span>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import { TestimonialSectionContent  } from '../constant';
//   interface Testimonial {
//     id: number;
//     name: string;
//     imgSrc: string;
//     message: string;
//   }
  
//   interface TestimonialSectionTestimonialSectionContent {
//     title: string;
//     subtitle: string;
//     testimonialGroups: Testimonial[][];
//   }
  
  
  
  </script>
  