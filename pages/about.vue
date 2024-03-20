<template>
  <section class="flex flex-col gap-10 p-10">
    <div class="flex flex-col gap-2">
      <p class="text-2xl font-semibold">{{ aboutData['our mission'].title }}</p>
      <p class="text-balance">{{ aboutData['our mission'].content }}</p>
    </div>

    <div class="flex flex-col gap-2">
      <p class="text-2xl font-semibold text-balance">{{ aboutData['our vision'].title }}</p>
      <p class="text-balance">{{ aboutData['our vision'].content }}</p>
    </div>

    <div class="flex flex-col justify-between md:flex-row">
      <div class="flex flex-col gap-2 md:w-[50%]">
        <p class="text-2xl font-semibold text-balance">{{ aboutData['our legal status'].title }}</p>
        <p class="text-balance">{{ aboutData['our legal status'].content }}</p>
      </div>
      <div class="md:w-[50%]">
        <Accordion :items="aboutData.accordion" />
      </div>
    </div>
  </section>
</template>

<script setup>
import aboutData from '~/data/about.json';
</script>