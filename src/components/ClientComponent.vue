<script setup>
import { getImageUrl } from '@/composables/getImageUrl'

const clientOpinions = [
  {
    text: 'Macrivate The most under-rated tools! Easy to setup, interactive analytics, great visualizations, and generous free tier. What more can you ask for!',
    name: 'Jeff Beck ',
    role: 'CEO, SomethingGood',
    img_url: 'client/Image-1.jpg'
  },
  {
    text: 'Macrivate feels like a partner, listening to our needs and making changes based on real users’ feedback',
    name: 'Virginia Morton ',
    role: 'CRO, Overpower',
    img_url: 'client/Image-2.jpg'
  },
  {
    text: 'The tool just keeps getting better and meets our needs more and more.',
    name: 'Sarah Hunt ',
    role: 'Head of Marketing, Goody',
    img_url: 'client/Image.jpg'
  }
]
</script>

<template>
  <section class="bg-primary text-white pt-[120px] pb-16">
    <div class="container mx-auto w-full flex justify-between">
      <div class="max-w-[652px] w-full">
        <p class="mb-8 font-semibold text-[48px] leading-[59px]">
          “This is one of many reasons why I found Metaview's notes helpful, but I was also blown
          away by how finely tuned the information is”
        </p>
        <div class="flex text-lg leading-[23px] items-center">
          <img class="mr-4" src="../assets/img/person.png" alt="" />
          <span class="font-semibold text-[#F3FB6E]">Mason Maldonado ·</span>
          <span class="opacity-50"> CEO, Amazing Company</span>
        </div>
      </div>
      <ul>
        <li
          v-for="clientOpinion in clientOpinions"
          :key="clientOpinion.name"
          class="pb-4 card-bottom mb-8"
        >
          <p class="text-lg font-normal mb-4">“{{ clientOpinion.text }}”</p>
          <div class="flex text-sm leading-[23px] items-center">
            <img class="mr-4 rounded-full" :src="getImageUrl(clientOpinion.img_url)" alt="" />
            <span class="font-semibold text-[#F3FB6E]">{{ clientOpinion.name }} · </span>
            <span class="opacity-50"> {{ clientOpinion.role }}</span>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.card-bottom {
  border-bottom: 1px solid rgba(255, 255, 255, 0.16);
}
</style>
