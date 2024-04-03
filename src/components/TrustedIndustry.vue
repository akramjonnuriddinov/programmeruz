<script setup>
import { getImageUrl } from '@/composables/getImageUrl'

const trusted_industries = [
  'trusted_industry/Logo-1.png',
  'trusted_industry/Logo-2.png',
  'trusted_industry/Logo-3.png',
  'trusted_industry/Logo-4.png',
  'trusted_industry/Logo-5.png'
]
</script>

<template>
  <div class="container mx-auto px-5">
    <div class="flex items-center justify-between">
      <h2 class="mr-5 whitespace-nowrap font-medium text-base leading-5 text-[#23232D]">
        Trusted by global industry leader
      </h2>
      <div class="flex justify-between rounded-full py-12 px-[72px]">
        <img
          v-for="trusted_industry in trusted_industries"
          :key="trusted_industry"
          :src="getImageUrl(trusted_industry)"
          :alt="trusted_industry"
          class="mr-4 opacity-50"
        />
      </div>
    </div>
  </div>
</template>
