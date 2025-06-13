<script></script>
<template>
  <div>
    <div
      class="bg-[url('/assets/images/h1_hero.png')] h-64 w-full bg-cover bg-center"
    >
      <!-- nav bar  -->
      <nav class="flex justify-around pt-9">
        <!-- logo  -->
        <img src="/assets/images/logo.png" class="pr-40" alt="" />
        <!-- pages  -->
        <ul class="flex gap-18 font-semibold cursor-pointer text-blue-950">
          <li class="hover:text-orange-400">
            <nuxt-link to="/"></nuxt-link>Home
          </li>
          <li class="hover:text-orange-400">
            <nuxt-link to="/about"></nuxt-link>About
          </li>
          <li class="hover:text-orange-400">
            <nuxt-link to="/blog"></nuxt-link>Blog
            <div class="bg-amber-50 w-[150px] h-[200px]">

            </div>
          </li>
          <li class="hover:text-orange-400">
            <nuxt-link to="/contact"></nuxt-link>Contact
          </li>
        </ul>
        <!-- contact button  -->
        <div
          class="w-[180px] h-[55px] bg-red-600 rounded-3xl text-center pt-3.5 text-white font-semibold mt-[-20px]"
        >
          0314-9535884
        </div>
      </nav>
    </div>
  </div>
</template>
