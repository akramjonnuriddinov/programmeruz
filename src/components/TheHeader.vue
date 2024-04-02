<script setup>
const links = [
  {
    id: '1',
    name: 'Products',
    path: '#'
  },
  {
    id: '2',
    name: 'Solutions',
    path: '#'
  },
  {
    id: '3',
    name: 'Customers',
    path: '#'
  },
  {
    id: '4',
    name: 'Pricing',
    path: '#'
  },
  {
    id: '5',
    name: 'About',
    path: '#'
  }
]
</script>

<template>
  <header>
    <nav class="text-black text-sm leading-[18px] border-[#D8D8D8] px-4 lg:px-6 py-4 border-b">
      <div class="flex flex-wrap justify-between items-center mx-auto max-w-screen-xl">
        <a href="#" class="flex items-center">
          <img src="@/assets/img/logo.svg" class="mr-3 h-6 sm:h-9" alt="Logo" />
        </a>
        <div class="flex font-semibold items-center lg:order-2">
          <a href="#" class="text-gray-800 px-4 lg:px-5 py-2 lg:py-2.5 mr-2">Log in</a>
          <button type="button" class="text-white text-sm bg-[#23232D] rounded-lg px-4 py-[11px]">
            Get Started
          </button>
        </div>
        <div class="hidden justify-between items-center w-full lg:flex lg:w-auto lg:order-1">
          <ul class="flex flex-col mt-4 lg:flex-row lg:space-x-8 lg:mt-0">
            <li v-for="link in links" :key="link.id">
              <router-link to="/" class="block py-2 pr-4 pl-3 lg:p-0">{{ link.name }}</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>
