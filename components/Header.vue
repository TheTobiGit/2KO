<template>
  <section class="flex items-center justify-between px-10 py-2 bg-white h-[7vh] md:h-[10vh]">
    <div class="flex items-center h-full">
      <img src="/images/logo.png" class="h-full md:h-[80%]" alt="">
    </div>
    <div class="hidden md:flex">
      <ul class="flex items-center gap-5 text-xl">
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/about">About Us</NuxtLink>
        <NuxtLink to="/contact">Contact Us</NuxtLink>
      </ul>
    </div>
  </section>
</template>

