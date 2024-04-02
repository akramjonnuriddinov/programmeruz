<script setup>
import ChevronIcon from '@/components/icons/ChevronIcon.vue'
</script>

<template>
  <div class="bg-[#23232D] pt-[100px]">
    <div
      class="container bg-[#FFFFFF0F] rounded-[64px] mx-auto flex flex-col items-center py-[100px]"
    >
      <div class="w-11/12 sm:w-2/3 mb-5 sm:mb-10">
        <h1 class="text-7xl text-center text-white font-semibold leading-[89px]">
          Simplify work and get more done now.
        </h1>
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
          class="ml-4 text-white bg-transparent transition border-[#ACACAC] duration-150 ease-in-out rounded-[20px] border py-5 px-10"
        >
          Take a Tour
        </button>
      </div>
    </div>
  </div>
</template>
