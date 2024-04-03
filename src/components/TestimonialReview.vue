<script setup>
import StarIcon from '@/components/icons/StarIcon.vue'
import { getImageUrl } from '@/composables/getImageUrl'

const reviews = [
  {
    img_url: 'reviewer/Image-1.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-2.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-3.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-4.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-5.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-6.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-7.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  },
  {
    img_url: 'reviewer/Image-8.jpg',
    name: 'Jeff Beck',
    role: 'CEO, SomethingGood',
    text: 'This is one of many reasons why I found Macrivate’s notes helpful, but I was also blown away by how finely tuned the information is'
  }
]
</script>

<template>
  <section class="bg-[#F3FB6E] py-[120px]">
    <div class="container mx-auto px-5">
      <div class="text-center mb-12 mx-auto w-full max-w-[750px] px-4">
        <span class="mb-4 text-base font-semibold leading-[20px] text-primary">Testimonials</span>
        <h2 class="text-[56px] text-black font-semibold leading-[69px]">Beloved by the best.</h2>
      </div>
      <ul class="flex flex-wrap gap-4 justify-between mb-16">
        <li
          v-for="review in reviews"
          :key="review.img_url"
          class="max-w-[273px] w-full flex flex-col justify-between rounded-3xl bg-white p-8"
        >
          <div class="flex gap-2">
            <star-icon v-for="i in 5" :key="i" />
          </div>

          <p class="my-3 mb-0 text-sm leading-[22px] font-normal tracking-wide text-black">
            {{ review.text }}
          </p>

          <div class="mt-6 flex items-center gap-6">
            <div class="h-10 w-10 overflow-hidden rounded-full shadow-sm outline-neutral-800">
              <div class="relative inline-block overflow-hidden rounded-lg border-neutral-800">
                <img
                  :src="getImageUrl(review.img_url)"
                  :alt="review.img_url"
                  width="50"
                  height="50"
                  class="inline-block"
                />
              </div>
            </div>
            <div class="text-sm">
              <p class="text-black font-semibold">{{ review.name }}</p>
              <p class="text-[#787878]">{{ review.role }}</p>
            </div>
          </div>
        </li>
      </ul>
      <div class="flex justify-center">
        <button class="text-primary font-semibold flex items-center">
          <span class="mr-2.5">View all testimonials</span>
          <img src="@/assets/img/circle-right.svg" alt="" />
        </button>
      </div>
    </div>
  </section>
</template>
