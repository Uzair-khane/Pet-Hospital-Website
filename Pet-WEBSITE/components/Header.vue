<script></script>
<template>
  <div>
    <div
      class="bg-[url('/assets/images/h1_hero.png')] h-64 w-full bg-cover bg-center "
    >
      <!-- nav bar  -->
      <nav  class="flex justify-around pt-9">
        <!-- logo  -->
        <img src="/assets/images/logo.png" alt="" />
        <!-- pages  -->
        <ul class="flex gap-18">
          <li><nuxt-link to="/"></nuxt-link>Home </li>
          <li><nuxt-link to="/about"></nuxt-link>About</li>
          <li><nuxt-link to="/blog"></nuxt-link>Blog</li>
          <li><nuxt-link to="/contact"></nuxt-link>Contact</li>
        </ul>
        <!-- contact button  -->
        <div>0314-9535884</div>
      </nav>
    </div>
  
  </div>
</template>
