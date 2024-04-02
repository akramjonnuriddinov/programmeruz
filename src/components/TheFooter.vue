<script setup>
const productLinks = [
  {
    name: 'Team Boards ',
    path: '#'
  },
  {
    name: 'Interactive Reports',
    path: '#'
  },
  {
    name: 'Group Analytics',
    path: '#'
  },
  {
    name: 'Data Integrations',
    path: '#'
  },
  {
    name: 'Security & Privacy',
    path: '#'
  },
  {
    name: 'Integration Directory',
    path: '#'
  }
]
const companyLinks = [
  {
    name: 'About Us',
    path: '#'
  },
  {
    name: 'Pricing',
    path: '#'
  },
  {
    name: 'Careers',
    path: '#'
  },
  {
    name: 'Press',
    path: '#'
  },
  {
    name: 'Contact',
    path: '#'
  }
]
const supportLinks = [
  {
    name: 'Contact Us',
    path: '#'
  },
  {
    name: 'Developer Docs',
    path: '#'
  },
  {
    name: 'Help Center',
    path: '#'
  }
]
const resourceLinks = [
  {
    name: 'Product Updates',
    path: '#'
  },
  {
    name: 'Customer Stories',
    path: '#'
  },
  {
    name: 'Testimonials',
    path: '#'
  },
  {
    name: 'Contact Us',
    path: '#'
  },
  {
    name: 'Blog',
    path: '#'
  },
  {
    name: 'FAQs',
    path: '#'
  }
]
</script>

<template>
  <footer class="text-white w-full bg-[#23232D]">
    <div class="w-full">
      <div
        class="container flex flex-col flex-wrap py-24 mx-auto md:items-center lg:items-start md:flex-row md:flex-no-wrap"
      >
        <div class="flex flex-wrap flex-grow mt-10 -mb-10 text-center md:mt-0 md:text-left">
          <div class="w-full px-4 lg:w-1/4 md:w-1/2">
            <h2
              class="mb-3 text-sm font-medium tracking-widest text-[#787878] uppercase title-font"
            >
              Product
            </h2>
            <nav class="mb-10 list-none">
              <li v-for="productLink in productLinks" :key="productLink.name" class="mt-3">
                <router-link to="/" class="cursor-pointer">{{ productLink.name }}</router-link>
              </li>
            </nav>
          </div>
          <div class="w-full px-4 lg:w-1/4 md:w-1/2">
            <h2
              class="mb-3 text-sm font-medium tracking-widest text-[#787878] uppercase title-font"
            >
              Company
            </h2>
            <nav class="mb-10 list-none">
              <li v-for="companyLink in companyLinks" :key="companyLink.name" class="mt-3">
                <router-link to="/" class="cursor-pointer">{{ companyLink.name }}</router-link>
              </li>
            </nav>
          </div>
          <div class="w-full px-4 lg:w-1/4 md:w-1/2">
            <h2
              class="mb-3 text-sm font-medium tracking-widest text-[#787878] uppercase title-font"
            >
              Support
            </h2>
            <nav class="mb-10 list-none">
              <li v-for="supportLink in supportLinks" :key="supportLink.name" class="mt-3">
                <router-link to="/" class="cursor-pointer">{{ supportLink.name }}</router-link>
              </li>
            </nav>
          </div>
          <div class="w-full px-4 lg:w-1/4 md:w-1/2">
            <h2
              class="mb-3 text-sm font-medium tracking-widest text-[#787878] uppercase title-font"
            >
              Recources
            </h2>
            <nav class="mb-10 list-none">
              <li v-for="resourceLink in resourceLinks" :key="resourceLink.name" class="mt-3">
                <router-link to="/" class="cursor-pointer">{{ resourceLink.name }}</router-link>
              </li>
            </nav>
          </div>
        </div>
      </div>
    </div>
    <div class="border-t pt-8 pb-16 border-[#585858]">
      <div class="w-full container mx-auto flex items-center">
        <a href="#" class="mr-8 flex items-center">
          <img src="@/assets/img/logo-white.svg" class="mr-3 h-6 sm:h-9" alt="Logo" />
        </a>
        <span class="text-sm text-[#949494]"
          >Copyright © 2023 Macrivate. All Rights Reserved.
        </span>
        <ul class="flex flex-wrap ml-auto items-center text-sm font-normal sm:mt-0">
          <li class="mr-10">
            <a href="#" class="hover:underline">Terms of Service</a>
          </li>
          <li>
            <a href="#" class="hover:underline">Privacy Policy</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>
