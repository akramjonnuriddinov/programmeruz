<script setup>
import { computed } from 'vue'
import { useRoute } from 'vue-router'
import TheHeader from '@/components/TheHeader.vue'

const route = useRoute()

const isHome = computed(() => {
  return route.name === 'home'
})
</script>

<template>
  <the-header :class="{ 'bg-[#D4F0F0]': isHome, 'bg-white': !isHome }" />
  <RouterView />
</template>
