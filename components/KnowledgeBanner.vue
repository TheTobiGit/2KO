<template>
  <section class="flex w-full p-10 text-white h-max">
    <div class="bg-[#1F2223] flex justify-evenly items-center w-full rounded-lg p-5 gap-5 flex-col md:flex-row">
      <img :src="knowledgeData.picture" alt="Knowledge Banner" class="w-[25vw] md:w-[10vw] h-auto" />
      <div class="flex flex-col gap-2 ">
        <p class="text-3xl font-semibold">{{ knowledgeData.title }}</p>
        <p>{{ knowledgeData.content }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import knowledgeData from '@/data/knowledgebanner.json';
</script>