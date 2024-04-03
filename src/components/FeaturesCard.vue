<script setup>
import { getImageUrl } from '@/composables/getImageUrl'

const features = [
  {
    img_url: 'feature_img/icon-1.svg',
    title: 'Engagement',
    text: 'Get feedback from everyone in the organization and find insights to build the culture you desire.'
  },
  {
    img_url: 'feature_img/icon-2.svg',
    title: 'Analytics',
    text: 'Utilize advanced people analytics to increase impact and innovation.'
  },
  {
    img_url: 'feature_img/icon-3.svg',
    title: 'Grow',
    text: 'Increase growth and engagement with Macrivate’s dynamic employee development tools.'
  },
  {
    img_url: 'feature_img/icon-4.svg',
    title: 'Performance',
    text: 'Identify your top performers, and equip every person to succeed with their work.'
  },
  {
    img_url: 'feature_img/icon-5.svg',
    title: 'Reimbursement',
    text: 'Engage and retain employees by connecting performance and compensation.'
  },
  {
    img_url: 'feature_img/icon-6.svg',
    title: 'OKR’s & Goals',
    text: 'Operate the business in a way that bridges the gap between people and operations.'
  }
]
</script>

<template>
  <ul class="flex flex-wrap justify-between items-center gap-x-6 gap-y-4">
    <li
      v-for="feature in features"
      :key="feature.title"
      class="flex items-center bg-white rounded-[48px] p-8 max-w-[558px] w-full"
    >
      <div class="rounded-full border p-6 mr-6">
        <img :src="getImageUrl(feature.img_url)" :alt="feature.title" />
      </div>
      <div>
        <h3 class="text-lg leading-6 text-black mb-2 font-semibold">{{ feature.title }}</h3>
        <p class="text-sm leading-[22px]">{{ feature.text }}</p>
      </div>
    </li>
  </ul>
</template>
