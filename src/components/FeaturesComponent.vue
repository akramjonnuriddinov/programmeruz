<script setup>
import FeaturesCard from '@/components/FeaturesCard.vue'
</script>

<template>
  <section class="bg-[#D4F0F0] py-[120px]">
    <div class="container mx-auto px-5">
      <div class="w-full max-w-[615px] flex flex-col mx-auto">
        <span class="mb-4 text-base text-center font-semibold leading-[20px] text-primary"
          >Features</span
        >
        <h2 class="mb-12 text-[56px] text-center text-black font-semibold leading-[69px]">
          We have more incredible features.
        </h2>
      </div>
      <features-card />
    </div>
  </section>
</template>
