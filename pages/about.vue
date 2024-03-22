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

    <div class="flex flex-col justify-between gap-5 md:flex-row md:gap-0">
      <div class="flex flex-col gap-2 md:w-[50%]">
        <p class="text-2xl font-semibold text-balance">{{ aboutData['our legal status'].title }}</p>
        <p class="text-balance">{{ aboutData['our legal status'].content }}</p>
      </div>
      <div class="md:w-[50%]">
        <Accordion :items="aboutData.accordion" />
      </div>
    </div>

  </section>

  <div class="flex py-4 pt-20 flex-col  gap-[3rem] h-max text-white bg-[#1F2223] rounded-t-[5rem] px-10">
    <p class="self-center text-5xl">Our Leadership</p>

    <div class="flex flex-col gap-10">
      <p class="self-center text-3xl">Board of Governors</p>
      <div class="flex flex-wrap gap-5">
        <div v-for="member in boardOfDirectors" :key="member.name" class="flex flex-col justify-center items-center text-balance gap-2  text-black bg-white rounded-lg w-full h-[15vh] md:w-[20vw] md:h-[20vh] mb-5 text-center p-4">
          <p class="text-xl font-semibold">{{ member.name }}</p>
          <p class="w-full">{{ member.position }}</p>
        </div>
      </div>
    </div>

    <div class="flex flex-col gap-10">
      <p class="self-center text-3xl">Management Team</p>
      <div class="flex flex-wrap gap-5">
        <div v-for="member in boardOfDirectors" :key="member.name" class="flex flex-col justify-center items-center text-balance gap-2  text-black bg-white rounded-lg w-full h-[15vh] md:w-[20vw] md:h-[20vh] mb-5 text-center p-4">
          <p class="text-xl font-semibold">{{ member.name }}</p>
          <p class="w-full">{{ member.position }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import aboutData from '~/data/about.json';
import leadershipData from '~/data/leadership.json';

const boardOfDirectors = leadershipData.boardOfDirectors;
const managementTeam = leadershipData.managementTeam;
</script>