<script setup>
import { useImage } from '~/composables/useImage.ts'

const title = ref('Palette Pilot - Generate Awesome Color Palette for you UI')
const description = ref('Explore Palette Pilot magic: transforming your images into color palettes and giving UI ideas. Perfect for creatives')

useHead({
  bodyAttrs: {
    class:
      'text-black bg-white dark:bg-black dark:text-white transition-colors ease-in-out duration-200 2xl:overflow-hidden'
  }
})

useSeoMeta({
  title: title,
  description: description,
  ogTitle: title,
  ogDescription: description,
  twitterTitle: title,
  twitterDescription: description,
  twitterCard: 'summary_large_image',
  icon: '/favicon.ico',
  lang: 'es',
})

defineOgImageComponent(
  'Palette',
  {
    title: title,
  }
)
</script>
<template>
  <Header />
  <NuxtPage />
</template>
<style>
@import url('primevue/resources/themes/aura-dark-noir/theme.css');
</style>
