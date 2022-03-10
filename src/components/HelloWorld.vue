<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="greetings-message">
      {{ msg }}
    </h1>
    <h3>
      You’ve successfully created a project with
      <a target="_blank" href="https://vitejs.dev/">Vite</a>
      +
      <a target="_blank" href="https://vuejs.org/"> Vue 3 </a>
      . What's next?
    </h3>
  </div>
</template>

<style scoped>
h1 {
  @apply font-medium text-4xl;
}

h3 {
  @apply text-xl;
}

.greetings h1,
.greetings h3 {
  @apply text-center mt-4;
}

.greetings-message {
  @apply text-green-500;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    @apply text-left;
  }
}
</style>
