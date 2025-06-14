<script setup>
import { ref } from "vue";

const isMobileMenuOpen = ref(false);
</script>

<template>
  <div>
    <nav class="flex items-center justify-between px-6 py-4">
      <!-- Logo -->
      <img src="/assets/images/logo.png" class="h-[50px]" alt="Logo" />

      <!-- Hamburger for Mobile -->
      <button
        class="text-white text-3xl md:hidden"
        @click="isMobileMenuOpen = !isMobileMenuOpen"
      >
        ☰
      </button>

      <!-- Desktop Menu -->
      <ul
        class="hidden md:flex gap-10 font-semibold cursor-pointer text-blue-950"
      >
        <li class="hover:text-orange-400">
          <nuxt-link to="/">Home</nuxt-link>
        </li>
        <li class="hover:text-orange-400">
          <nuxt-link to="/about">About</nuxt-link>
        </li>

        <li class="hover:text-orange-400 relative group">
          <nuxt-link to="/blog">Blog</nuxt-link>
          <!-- Dropdown -->
          <ul
            class="absolute left-0 top-full bg-amber-50 p-4 rounded-md mt-2 hidden group-hover:grid gap-2 w-40 transition-opacity duration-300"
          >
            <li><a href="">Blog</a></li>
            <li><a href="">Blog Details</a></li>
            <li><a href="">Element</a></li>
          </ul>
        </li>

        <li class="hover:text-orange-400">
          <nuxt-link to="/contact">Contact</nuxt-link>
        </li>
      </ul>

      <!-- Contact Button -->
      <div
        class="hidden md:block w-[180px] h-[55px] bg-red-600 rounded-3xl text-center pt-3.5 text-white font-semibold"
      >
        0314-9535884
      </div>
    </nav>

    <!-- Mobile Menu -->
    <div
      v-if="isMobileMenuOpen"
      class="md:hidden bg-amber-100 w-[355px] pt-10 h-[600px] transition duration-300 ease-in-out flex flex-col gap-[10px] text-blue-950 font-semibold px-6 py-4 space-y-4 bg"
    >
      <nuxt-link class="text-center" to="/" @click="isMobileMenuOpen = false"
        >Home</nuxt-link
      ><br />
      <nuxt-link
        class="text-center"
        to="/about"
        @click="isMobileMenuOpen = false"
        >About</nuxt-link
      ><br />
      <nuxt-link
        class="text-center"
        to="/blog"
        @click="isMobileMenuOpen = false"
        >Blog</nuxt-link
      ><br />
      <nuxt-link
        class="text-center"
        to="/contact"
        @click="isMobileMenuOpen = false"
        >Contact</nuxt-link
      >
    </div>
  </div>
</template>
