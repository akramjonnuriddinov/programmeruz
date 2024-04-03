<template>
  <section class="bg-[#F3FB6E] py-[120px]">
    <div class="container mx-auto px-5">
      <div class="text-center mb-12 mx-auto w-full max-w-[750px] px-4">
        <span class="mb-4 text-base font-semibold leading-[20px] text-primary">Testimonials</span>
        <h2 class="text-[56px] text-black font-semibold leading-[69px]">Beloved by the best.</h2>
      </div>
      <div
        class="flex flex-col justify-between rounded-3xl bg-white p-8 shadow-sm max-w-sm mx-auto mt-24"
      >
        <div class="text-[#FEBC62] flex gap-2">
          <svg
            v-for="i in 5"
            :key="i"
            xmlns="http://www.w3.org/2000/svg"
            class="text-[#FEBC62]"
            width="20"
            height="20"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="none"
            fill="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
            <path
              d="M12 17.75l-6.172 3.245l1.179 -6.873l-5 -4.867l6.9 -1l3.086 -6.253l3.086 6.253l6.9 1l-5 4.867l1.179 6.873z"
            ></path>
          </svg>
        </div>

        <p class="my-3 mb-0 text-sm leading-[22px] font-normal tracking-wide text-black">
          I've been using XYZ for over a year now and their customer service is excellent! Whenever
          I have a question, the team is always available and willing to help. Highly recommend!
        </p>

        <div class="mt-6 flex items-center gap-6">
          <div class="h-10 w-10 overflow-hidden rounded-full shadow-sm outline-neutral-800">
            <div class="relative inline-block overflow-hidden rounded-lg border-neutral-800">
              <img
                alt=""
                src="https://randomuser.me/api/portraits/women/2.jpg"
                width="50"
                height="50"
                decoding="async"
                data-nimg="1"
                class="inline-block"
                loading="lazy"
                style="color: transparent"
              />
            </div>
          </div>
          <div class="text-sm">
            <p class="text-black font-semibold">Melissa Smith</p>
            <p class="text-[#787878]">Marketing Manager</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
