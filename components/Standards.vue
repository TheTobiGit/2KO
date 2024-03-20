<template>
  <section class="flex flex-col gap-10 p-10 h-max">
    <p class="text-3xl font-semibold">Our Standards</p>
    <div class="flex flex-col flex-wrap justify-between gap-10 md:flex-row lg:gap-0">
      <div class="flex flex-col gap-5 h-max w-full md:max-w-[40vw] mb-10" v-for="standard in standardsList" :key="standard.title">
        <img :src="standard.picture" alt="" class="w-[10vw] h-auto" />
        <p class="font-semibold">{{ standard.title }}</p>
        <p class="text-balance">{{ standard.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import standardsData from '@/data/standards.json';

const { standards: standardsList } = standardsData;
</script>