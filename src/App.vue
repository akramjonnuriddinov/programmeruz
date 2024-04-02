<script setup>
import { computed } from 'vue'
import { useRoute } from 'vue-router'
import TheHeader from '@/components/TheHeader.vue'
import TheFooter from '@/components/TheFooter.vue'

const route = useRoute()

const isHome = computed(() => {
  return route.name === 'home'
})
</script>

<template>
  <the-header :class="{ 'bg-[#D4F0F0]': isHome, 'bg-white': !isHome }" />
  <RouterView />
  <the-footer />
</template>
