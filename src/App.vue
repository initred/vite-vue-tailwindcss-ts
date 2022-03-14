<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router"
import HelloWorld from "@/components/HelloWorld.vue"
import TheLogo from "@/components/TheLogo.vue"
</script>

<template>
  <header>
    <div class="wrapper">
      <TheLogo />

      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
#app {
  @apply max-w-7xl grid grid-cols-1 gap-8 mx-auto p-8;
}

header {
  @apply max-h-screen;
}

header .wrapper {
  @apply space-y-14;
}

nav {
  @apply w-full flex justify-center divide-x my-8 ml-0;
}

nav a {
  @apply inline-block px-4;
}

nav a.router-link-exact-active {
  @apply text-[#2c3e50];
}

nav a.router-link-exact-active:hover {
  @apply bg-transparent;
}

@media screen(lg) {
  body {
    @apply flex place-items-center;
  }

  #app {
    @apply grid grid-cols-2 gap-8 px-8;
  }

  header {
    @apply flex place-items-center;
  }

  header .wrapper {
    @apply place-content-start place-items-start flex-wrap space-y-10;
  }

  nav {
    @apply w-full justify-start -ml-4;
  }
}
</style>
