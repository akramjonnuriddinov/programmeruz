<script setup>
import ChevronIcon from '@/components/icons/ChevronIcon.vue'
import { getImageUrl } from '@/composables/getImageUrl.js'

const integrations = [
  'integration/Logo-1.png',
  'integration/Logo-2.png',
  'integration/Logo-3.png',
  'integration/Logo-4.png',
  'integration/Logo-5.png',
  'integration/Logo-6.png',
  'integration/Logo-7.png',
  'integration/Logo-8.png'
]
</script>

<template>
  <section class="bg-[#F9F9F9] pt-[120px]">
    <div class="text-center mx-auto w-full max-w-[750px] px-4">
      <span class="mb-4 text-base font-semibold leading-[20px] text-primary">Integration</span>
      <h2 class="mb-6 text-[56px] text-black font-semibold leading-[69px]">
        Integrate your favorite software seamlessly.
      </h2>
      <div class="flex justify-center">
        <button
          class="bg-primary flex items-center transition duration-150 ease-in-out rounded-[20px] text-white py-2 pl-10 pr-2"
        >
          Explore our integrations
          <div class="ml-8 py-4 rounded-2xl px-[18px] bg-white">
            <chevron-icon class="w-2 text-[#23232D] h-4" />
          </div>
        </button>
      </div>
    </div>
    <ul class="flex items-center justify-between w-full pt-[72px] pb-[120px]">
      <li
        v-for="integration in integrations"
        :key="integration"
        class="p-8 integration bg-white rounded-3xl"
      >
        <img :src="getImageUrl(integration)" :alt="integration" />
      </li>
    </ul>
  </section>
</template>

<style scoped>
.integration {
  box-shadow: 0px 12px 72px 0px #00000014;
}
</style>
