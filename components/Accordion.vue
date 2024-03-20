<template>
  <div>
    <div v-for="(item, index) in items" :key="index">
      <div @click="toggleAccordion(index)" class="bg-gray-100 border-b">
        <div class="flex items-center justify-between p-4 cursor-pointer">
          <div class="font-semibold">{{ item.title }}</div>
          <div v-if="activeIndex === index">
            <svg
              class="w-6 h-6 transform rotate-180"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              />
            </svg>
          </div>
          <div v-else>
            <svg
              class="w-6 h-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              />
            </svg>
          </div>
        </div>
      </div>
      <div v-if="activeIndex === index" class="p-4 bg-white">
        {{ item.content }}
      </div>
    </div>
  </div>
</template>

<script setup>

const activeIndex = ref(null);

const toggleAccordion = (index) => {
  if (activeIndex.value === index) {
    activeIndex.value = null;
  } else {
    activeIndex.value = index;
  }
};

const props = defineProps({
  items: {
    type: Array,
    required: true
  }
});
</script>