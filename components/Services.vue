<template>
  <section class="flex flex-col gap-10 p-10 h-max">
    <p class="text-3xl font-semibold">Services</p>
    <div class="flex flex-col flex-wrap justify-between gap-10 md:flex-row lg:gap-0">
      <div class="flex flex-col w-full md:max-w-[40vw] h-max gap-5" v-for="service in serviceList" :key="service.title">
        <img :src="service.picture" alt="" class="w-[10vw] h-auto" />
        <p class="font-semibold">{{ service.title }}</p>
        <p>{{ service.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import serviceData from '@/data/services.json';

const { services: serviceList } = serviceData;
</script>