<template>
  <div>
    <Navbar />
    <section class="relative h-[500px] w-full flex items-center justify-start">
      <div
        class="absolute inset-0 bg-cover bg-center"
        style="background-image: url('/images/restaurant.jpg');"
      ></div>
      <div class="absolute inset-0 backdrop-blur-sm bg-black/40"></div>
      <div class="relative z-10 text-white max-w-xl ml-10">
        <p class="text-lg opacity-90">Welcome to foodify~~  </p>
        <h1 class="text-5xl font-bold leading-tight mt-2">
          Your Fast - Food Innovation Partner
        </h1>
        <p class="mt-4 text-gray-200">
          Delivering delicious, efficient, and scalable solutions that keep your quick-service brand ahead of the competition.
        </p>
        <button
          class="mt-6 bg-orange-500 hover:bg-orange-600 text-white px-6 py-3 rounded-lg font-semibold"
        >
          Contact Us
        </button>
      </div>
    </section>
    <section
      class="relative py-20 px-6 bg-cover bg-center"
      :style="{ backgroundImage: `url(${overviewBg})` }"
    >
      <div class="absolute inset-0 bg-black/40 backdrop-blur-sm"></div>
      <div class="relative max-w-6xl mx-auto text-white">
        <h1 class="text-4xl font-bold text-center mb-6">Company Overview</h1>
        <p class="text-center text-lg max-w-2xl mx-auto mb-12">
          Your trusted partner in modern quick-service food innovation.
        </p>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-10 items-center">
          <div>
            <h2 class="text-2xl font-semibold text-orange-400 mb-4">
             foodify
            </h2>
            <p class="mb-4">
              Foodify is a forward-thinking fast-food company committed to delivering delicious, high-quality meals with speed, consistency, and innovation. Built on a passion for great taste and efficient service, Foodify continues to redefine the fast-food experience for today’s fast-moving world.
            </p>
            <p>
              Embracing the slogan “Fast. Fresh. Future-Ready.”, Foodify embodies a commitment to quality, speed, and continuous innovation. From product development to kitchen workflow optimization, we strive to deliver an exceptional dining experience.
            </p>
          </div>
          <div class="flex justify-center">
            <div class="bg-white shadow-xl rounded-2xl p-8">
              <img :src="foodifyLogo" class="w-48 h-48 object-contain" />
            </div>
          </div>
        </div>
      </div>
    </section>
    <Footer />
  </div>
</template>
<script setup>
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue'

import overviewBg from '@/assets/images/overview-bg.jpg'
import foodifyLogo from '@/assets/images/foodifylogo.jpg' 
</script>
