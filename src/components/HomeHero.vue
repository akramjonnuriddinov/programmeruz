<script setup>
import ChevronIcon from '@/components/icons/ChevronIcon.vue'
</script>

<template>
  <div class="bg-[#D4F0F0]">
    <div class="container mx-auto px-5 flex flex-col items-center pt-[72px] pb-[54px]">
      <div class="w-11/12 sm:w-2/3 mb-5 sm:mb-10">
        <h1 class="text-7xl text-center text-black font-semibold leading-[89px]">
          Your ultimate SaaS all-in-one solution.
        </h1>
        <p class="mt-4 mx-auto text-center text-lg max-w-[500px] w-full">
          Boost conversions, engage users, and retain customers with powerful, self-service
          analytics.
        </p>
      </div>
      <div class="flex font-medium text-lg leading-[23px] justify-center mb-[72px]">
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
      <!-- DIAGRAM -->
      <div class="w-full dashboard">
        <div class="first-area bg-white rounded-3xl p-6 pt-[22px]">
          <div class="flex items-center justify-between mb-[26px]">
            <button>
              <img src="../assets/img/dashboard/left-icon.svg" alt="" />
            </button>
            <span>December 2023</span>
            <button>
              <img src="../assets/img/dashboard/right-icon.svg" alt="" />
            </button>
          </div>
          <div class="flex justify-center mb-[28px]">
            <img src="../assets/img/dashboard/item1.png" alt="" />
          </div>
          <ul class="flex items-center justify-center">
            <li class="flex items-center mr-6">
              <span class="flex w-2 h-2 rounded-full bg-primary mr-[6px]"></span>
              <span class="text-sm">Desktops</span>
            </li>
            <li class="flex items-center mr-6">
              <span class="flex w-2 h-2 rounded-full bg-[#FFCA82] mr-[6px]"></span>
              <span class="text-sm">Mobiles</span>
            </li>
            <li class="flex items-center mr-6">
              <span class="flex w-2 h-2 rounded-full bg-[#F7A7E9] mr-[6px]"></span>
              <span class="text-sm">Tablets</span>
            </li>
          </ul>
        </div>
        <div class="second-area bg-white rounded-3xl p-6 pt-[22px]">
          <h3 class="text-[#30323F] font-semibold text-base leading-[19px]">Convertion Rate</h3>
          <div class="text-sm flex items-center mb-8">
            <span class="font-bold text-[32px] leading-[38.73px] text-[#30323F] mr-4">0.87%</span>
            <div class="flex items-center">
              <div class="flex items-center mr-1 text-[#57C347]">
                <img src="../assets/img/up-icon.svg" alt="" />
                <span>2.5%</span>
              </div>
              <span class="text-[#8E8F98]">than last week</span>
            </div>
          </div>
          <div class="flex justify-center">
            <img src="../assets/img/dashboard/item2.png" alt="" />
          </div>
        </div>
        <div class="third-area bg-white rounded-3xl p-6 pt-[22px]">
          <div class="mb-4">
            <div class="text-sm flex items-center justify-between mb-8">
              <div>
                <h3 class="text-[#30323F] font-semibold text-base leading-[19px]">
                  Convertion Rate
                </h3>
                <div class="flex">
                  <div class="flex items-center mr-1 text-[#57C347]">
                    <img src="../assets/img/up-icon.svg" alt="" />
                    <span>2.5%</span>
                  </div>
                  <span class="text-[#8E8F98]">than last week</span>
                </div>
              </div>
              <span class="font-bold text-[32px] leading-[38.73px] text-[#30323F] ml-4">0.87%</span>
            </div>
          </div>
          <div class="flex justify-center">
            <img src="../assets/img/dashboard/item3.png" alt="" />
          </div>
        </div>
        <div class="fourth-area bg-white rounded-3xl p-6 pt-[22px]">
          <div class="flex justify-between items-center pb-6 border-b border-[#EBECEF]">
            <div>
              <div class="flex items-center mb-2">
                <span class="font-bold text-[32px] leading-[38.73px] text-[#30323F] mr-2"
                  >1,203</span
                >
                <div class="flex items-center mr-1 text-[#57C347]">
                  <img src="../assets/img/up-icon.svg" alt="" />
                  <span>2.5%</span>
                </div>
              </div>
              <span class="text-[#8E8F98]">Visitor this year</span>
            </div>
            <img src="../assets/img/dashboard/item4.png" alt="" />
          </div>
          <div class="flex justify-between items-center pt-6">
            <div>
              <div class="flex items-center mb-2">
                <span class="font-bold text-[32px] leading-[38.73px] text-[#30323F] mr-2">672</span>
                <div class="flex items-center mr-1 text-[#FF4B4B]">
                  <img src="../assets/img/down-icon.svg" alt="" />
                  <span>2.5%</span>
                </div>
              </div>
              <span class="text-[#8E8F98]">Visitor this month</span>
            </div>
            <img src="../assets/img/dashboard/item5.png" alt="" />
          </div>
        </div>
        <div class="fifth-area bg-white rounded-3xl p-6 pt-[22px]">
          <span class="text-[#8E8F98] mb-7">Pageviews</span>
          <div class="flex items-center justify-between">
            <div class="flex items-center mb-2">
              <span class="font-bold text-[32px] leading-[38.73px] text-[#30323F] mr-2">1,203</span>
              <div class="flex items-center mr-1 text-[#57C347]">
                <img src="../assets/img/up-icon.svg" alt="" />
                <span>2.5%</span>
              </div>
            </div>
            <img src="../assets/img/dashboard/eye.png" alt="" />
          </div>
        </div>
      </div>
      <!-- /DIAGRAM -->
    </div>
  </div>
</template>

<style scoped>
.dashboard {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  grid-template-areas:
    'first-area second-area forth-area'
    'first-area third-area fifth-area'
    '. . .';
}

.first-area {
  grid-area: first-area;
}
.second-area {
  grid-area: second-area;
}
.third-area {
  grid-area: third-area;
}
.forth-area {
  grid-area: forth-area;
}
.fifth-area {
  grid-area: fifth-area;
}
</style>
