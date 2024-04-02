<script setup>
import { getImageUrl } from '@/composables/getImageUrl'

const blogs = [
  {
    title: 'The state of product analytics',
    text: 'The most successful companies today value, analyze, and learn from their customer data. And two tools in many of these …',
    topic: 'Analytics',
    time: 'Oct 3 ',
    createdAt: '7 min ',
    img_url: 'blog/blog1.png'
  },
  {
    title: 'Macrivate Launches Technology Partnership with UKG',
    text: 'The most successful companies today value, analyze, and learn from their customer data. And two tools in many of these …',
    topic: 'Analytics',
    time: 'Oct 3 ',
    createdAt: '8 min ',
    img_url: 'blog/blog2.png'
  }
]
</script>

<template>
  <section class="py-[120px]">
    <div class="container mx-auto">
      <div class="flex mb-16 justify-between items-end">
        <h2 class="text-[56px] text-black font-semibold leading-[69px]">News & Updates.</h2>
        <button class="text-primary font-semibold flex items-center">
          <span class="mr-2.5">View all articles</span>
          <img src="@/assets/img/circle-right.svg" alt="" />
        </button>
      </div>
      <ul class="mx-auto flex justify-between gap-[30px]">
        <li
          v-for="blog in blogs"
          :key="blog.title"
          class="max-w-[555px] w-full flex flex-col rounded-[48px] bg-[#F9F9F9] shadow-md"
        >
          <a href="#">
            <img class="rounded-t-[48px]" :src="getImageUrl(blog.img_url)" alt="" />
          </a>
          <div class="p-10 pt-8 flex flex-col h-full">
            <div class="mb-3">
              <span class="text-primary mr-8">Analytics</span>
              <span
                ><span>{{ blog.createdAt }}</span> · <span>{{ blog.time }}</span> read</span
              >
            </div>
            <a href="#">
              <h5 class="mb-3 text-2xl font-semibold text-black">{{ blog.title }}</h5>
            </a>
            <p class="text-base leading-[26px] mb-14 font-normal text-[#585858]">
              {{ blog.text }}
            </p>
            <a class="underline mt-auto text-primary text-base leading-5" href="#"
              >View all articles</a
            >
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>
