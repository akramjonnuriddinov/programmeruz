<template>
  <section class="bg-tg-white py-10">
    <div class="container mx-auto w-full px-5">
      <div class="flex items-center">
        <div class="relative z-10">
          <img class="w-[555px] h-[660px]" src="@/assets/img/working-girl.jpg" alt="" />
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

<script setup>
import { ref } from 'vue'

const aboutContents = ref(['Organize your data', 'Work with any team', 'Business analytics'])
</script>
