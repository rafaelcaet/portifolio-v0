<template>
  <div class="h-screen flex flex-col">
    <div
      class="p-2 my-2 rounded-full hover:bg-blue-50 w-min dark:hover:bg-white/20"
      :class="defaultTransition"
    >
      <nuxt-link to="/">
        <div class="w-8 h-8">
          <LogoSocialMedia />
        </div>
      </nuxt-link>
    </div>
    <HomeIcon />
  </div>
</template>
<script setup>
import { HomeIcon } from "@heroicons/vue/solid";
const { defaultTransition } = useTailwindConfig();
</script>
