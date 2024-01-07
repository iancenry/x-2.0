<template>
  <div class="flex flex-col h-screen">
    <div
      class="p-2 my-2 hover:scale-105 rounded-full w-min hover:bg-blue-50 dark:hover:bg-white/20"
      :class="defaultTransition"
    >
      <NuxtLink to="/">
        <div class="h-8 w-8">
          <LogoTwitter />
        </div>
      </NuxtLink>
    </div>
    <HomeIcon />
  </div>
</template>

<script setup>
import { HomeIcon } from '@heroicons/vue/solid';
const { defaultTransition } = useTailwindConfig();
</script>
