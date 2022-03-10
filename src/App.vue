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
        <RouterLink to="/"> Home </RouterLink>
        <RouterLink to="/about"> About </RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
