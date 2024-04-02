<script setup>
import ChevronIcon from '@/components/icons/ChevronIcon.vue'
</script>

<template>
  <div class="bg-[#D4F0F0]">
    <div class="container mx-auto flex flex-col items-center py-[72px]">
      <div class="w-11/12 sm:w-2/3 mb-5 sm:mb-10">
        <h1 class="text-7xl text-center text-black font-semibold leading-[89px]">
          Your ultimate SaaS all-in-one solution.
        </h1>
        <p class="mt-4 mx-auto text-center text-lg max-w-[500px] w-full leading-7">
          Boost conversions, engage users, and retain customers with powerful, self-service
          analytics.
        </p>
      </div>
      <div class="flex font-medium text-lg leading-[23px] justify-center">
        <button
          class="bg-primary flex items-center transition duration-150 ease-in-out rounded-[20px] text-white py-2 pl-10 pr-2"
        >
          Get Started
          <div class="ml-8 py-4 rounded-2xl px-[18px] bg-white">
            <chevron-icon class="w-2 text-[#23232D] h-4" />
          </div>
        </button>
        <button
          class="ml-4 text-black bg-transparent transition border-[#ACACAC] duration-150 ease-in-out rounded-[20px] border py-5 px-10"
        >
          Take a Tour
        </button>
      </div>
    </div>
  </div>
</template>
