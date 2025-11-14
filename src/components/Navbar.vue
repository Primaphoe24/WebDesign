<template>
  <nav class="relative p-4 bg-linear-to-r from-orange-400 via-orange-500 to-orange-600 shadow-xl flex justify-between text-white overflow-hidden">
  <div class="absolute top-0 left-0 right-0 h-[3px] bg-white/30"></div>

  <h1 class="text-2xl font-bold relative">foodify</h1>

  <div class="flex gap-6 relative">
    <router-link to="/" class="hover:text-yellow-200 transition">Home</router-link>
    <router-link to="/contact" class="hover:text-yellow-200 transition">Contact</router-link>
  </div>

</nav>

</template>
