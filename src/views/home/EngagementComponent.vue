<script setup>
import { ref } from 'vue'

const aboutContents = ref(['Organize your data', 'Work with any team', 'Business analytics'])
</script>

<template>
  <section class="bg-tg-white py-10">
    <div class="container mx-auto w-full px-5">
      <div class="flex items-center">
        <div class="relative z-10">
          <img class="w-[555px] h-[660px]" src="@/assets/img/working-girl.jpg" alt="" />
          <div
            class="flex rounded-full bg-white w-full max-w-[330px] p-6 absolute bottom-16 left-1/2 -translate-x-1/2 card"
          >
            <img class="mr-4" src="@/assets/img/pie39.png" alt="" />
            <div>
              <h5 class="text-sm font-medium mb-2">
                <span class="font-semibold">Significantly</span> exceeded business goals
              </h5>
              <p class="text-xs">Past 12 month</p>
            </div>
          </div>
        </div>
        <div class="relative ml-12 w-full max-w-[600px] px-4">
          <span class="mb-4 text-base font-semibold leading-[20px] text-primary">Engagement</span>
          <h2 class="mb-6 text-[56px] text-black font-semibold leading-[69px]">
            Get to know your employees' voices at scale.
          </h2>
          <p class="mb-8 text-lg">
            Listen, reflect, and respond to engagement feedback to retain top talent as your
            business grows, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
          <ul class="mb-14">
            <li
              v-for="aboutContent in aboutContents"
              :key="aboutContent"
              class="mb-6 flex items-center"
            >
              <div class="mr-3 w-6 h-6 flex items-center justify-center rounded-full bg-[#D4F0F0]">
                <img class="" src="@/assets/img/check.svg" alt="" />
              </div>
              <p class="leading-[1.8] text-black">
                {{ aboutContent }}
              </p>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.card {
  box-shadow: 12px 24px 48px 0px #0000001f;
}
</style>
