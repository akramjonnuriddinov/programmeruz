<template>
  <section class="bg-tg-white py-10">
    <div class="container mx-auto px-5 w-full">
      <div class="w-full flex items-center gap-x-[128px]">
        <div class="relative w-full max-w-[457px] px-4">
          <span class="mb-4 text-base font-semibold leading-[20px] text-primary">Performance</span>
          <h2 class="mb-6 text-[56px] text-black font-semibold leading-[69px]">
            Performance management employees love.
          </h2>
          <p class="mb-8 text-lg">
            Identify your top performers, and equip every person to succeed with their work. Lorem
            ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
            labore et dolore magna aliqua.
          </p>
          <div>
            <div class="text-black flex mb-4 items-center">
              <span class="font-semibold text-[32px] leading-[39px] mr-6">1.8x</span>
              <p class="text-lg leading-[23px]">User base growth</p>
            </div>
            <div class="text-black flex items-center">
              <span class="font-semibold text-[32px] leading-[39px] mr-6">22%</span>
              <p class="text-lg leading-[23px]">Increase in retention</p>
            </div>
          </div>
        </div>
        <div class="relative z-10">
          <img class="w-[555px] h-[660px]" src="@/assets/img/working-girl-2.jpg" alt="" />
          <div
            class="flex rounded-3xl justify-between flex-row-reverse bg-white w-full max-w-[330px] p-6 absolute bottom-6 left-6 card"
          >
            <img class="ml-4" src="@/assets/img/bar.png" alt="" />
            <div class="text-[#23232D]">
              <h5 class="text-sm font-semibold mb-2">Order Quantity</h5>
              <span class="font-bold text-[48px] leading-[63px]">1.230</span>
              <div class="text-xs flex items-center">
                <span class="text-[#FF4B4B] flex items-center mr-2">
                  <img src="../assets/img/down-icon.svg" alt="" />
                  <span>2.5%</span>
                </span>
                than last week
              </div>
            </div>
          </div>
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
