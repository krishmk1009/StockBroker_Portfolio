<!-- src/components/Navbar.vue -->
<template>
  <nav class="relative z-10 flex justify-between items-center p-6">
    <div class="flex items-center space-x-4">
      <!-- Logo -->
      <div class="text-white text-2xl font-bold">Logo</div>
      <!-- Nav Links (Left) -->
      <div class="hidden md:flex space-x-4">
        <a href="#" class="text-white hover:text-gray-300">Home</a>
        <a href="#" class="text-white hover:text-gray-300">About</a>
        <a href="#" class="text-white hover:text-gray-300">Services</a>
      </div>
    </div>
    <!-- Nav Links (Right) -->
    <div class="flex items-center space-x-4">
      <a href="#" class="text-white hover:text-gray-300">Portfolio</a>
      <a href="#" class="text-white hover:text-gray-300">Contact</a>
      <button class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-700">Get Started</button>
    </div>
  </nav>
</template>

<script>

</script>


