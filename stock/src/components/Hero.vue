<!-- src/components/HeroSection.vue -->
<template>
  <div class="relative h-screen-80 bg-cover bg-center flex flex-col" :style="{ backgroundImage: `url(https://images.unsplash.com/photo-1560221328-12fe60f83ab8?q=80&w=2948&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D` }">
    <!-- Background Overlay with Low Opacity -->
    <div class="absolute inset-0 bg-gray-900 bg-opacity-70 z-0"></div>
    
    <!-- Navbar -->
    <nav class="relative z-10 flex justify-between items-center p-6">
      <div class="flex items-center space-x-4">
        <!-- Logo -->
        <img :src="Icon1" alt="logo" />
        <!-- <img :src="NavbarContent.logo" alt="NavbarContent.logo"/> -->
        <!-- Nav Links (Left) -->
        <div class="hidden md:flex space-x-4">
          <a href="#" class="text-white hover:text-gray-300">Home</a>
          <a href="#" class="text-white hover:text-gray-300">Our Services</a>
          <a href="#" class="text-white hover:text-gray-300">About Us</a>
        </div>
      </div>
      <!-- Nav Links (Right) -->
      <div class="flex items-center space-x-4">
        <a href="#" class="text-white hover:text-gray-300">Testimonial</a>
        <a href="#" class="text-white hover:text-gray-300">Contact</a>
        <button class="bg-green-600 text-white px-4 py-2 rounded-full hover:bg-blue-700">Get Started</button>
      </div>
    </nav>

    <!-- Hero Content -->
    <div class="relative z-10 flex flex-1 items-center justify-center text-center">
      <div class="text-white">
        <h1 class="text-5xl font-bold mb-4">Welcome to Our Website</h1>
        <p class="text-xl mb-8 w-3/5 mx-auto">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Necessitatibus minus perferendis vel, unde animi aperiam alias inventore,
        </p>
        <button class="bg-red-500 text-white px-6 py-3 rounded-full hover:bg-red-700">Learn More</button>
      </div>
    </div>
  </div>
</template>

<script>
import Icon1 from '../assets/icon1.png';
</script>

<style scoped>
.h-screen-80 {
  height: 80vh;
}
</style>
