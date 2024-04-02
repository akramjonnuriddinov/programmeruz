<template>
  <section class="py-[100px]">
    <div class="mx-auto container px-6 text-black">
      <div class="mx-auto flex items-center">
        <p class="text-2xl max-w-[200px] w-full">The work we have done so far</p>
        <div
          class="mx-auto grid grid-cols-1 gap-0.5 rounded-2xl text-center sm:grid-cols-2 lg:grid-cols-4"
        >
          <div v-for="work in works" :key="work.id" class="flex gap-y-2 flex-col p-8">
            <h4 class="text-lg text-[#787878] leading-[23px]">
              {{ work.title }}
            </h4>
            <p class="order-first text-5xl font-semibold leading-[59px]">
              {{ work.count }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const works = ref([
  {
    id: '1',
    title: 'User growth',
    count: '32%'
  },
  {
    id: '2',
    title: 'Churn rate',
    count: '10%'
  },
  {
    id: '3',
    title: 'Revenue growth',
    count: '18%'
  },
  {
    id: '4',
    title: 'Engagement rate',
    count: '42%'
  }
])
</script>
