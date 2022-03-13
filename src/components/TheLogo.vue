<script setup lang="ts">
import LogoVite from "@/assets/logo-vite.svg?component"
import LogoVue from "@/assets/logo-vue.svg?component"
import LogoTailwindcss from "@/assets/logo-tailwindcss.svg?component"
import LogoEslint from "@/assets/logo-eslint.svg?component"
import LogoPrettier from "@/assets/logo-prettier.svg?component"
import LogoTypescript from "@/assets/logo-typescript.svg?component"
</script>

<template>
  <div class="logo">
    <i><LogoVite /></i>
    <i><LogoVue /></i>
    <i><LogoTailwindcss /></i>
    <i><LogoPrettier /></i>
    <i><LogoEslint /></i>
    <i><LogoTypescript /></i>
  </div>
</template>

<style scoped>
.logo {
  @apply grid grid-cols-3 place-content-center place-items-center gap-8;
}

.logo i > * {
  @apply w-16 h-auto fill-current;
}
</style>
