<script setup>
import ChevronIcon from '@/components/icons/ChevronIcon.vue'
</script>

<template>
  <div class="">
    <div class="container mx-auto px-5 pt-[72px]">
      <div class="flex mb-[72px]">
        <h1 class="text-7xl max-w-[652px] w-full mr-[30px] text-black font-semibold leading-[89px]">
          A powerful tool you'll love to use.
        </h1>
        <div class="flex flex-col">
          <p class="mb-12 text-lg max-w-[420px] w-full">
            Boost conversions, engage users, and retain customers with powerful, self-service
            analytics.
          </p>
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
              class="ml-6 text-black bg-transparent transition border-[#ACACAC] duration-150 ease-in-out rounded-[20px] border py-5 px-10"
            >
              Take a Tour
            </button>
          </div>
        </div>
      </div>
      <img src="../assets/img/dashboard2.png" alt="" />
    </div>
  </div>
</template>
