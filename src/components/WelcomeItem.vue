<template>
  <div class="item">
    <i>
      <slot name="icon" />
    </i>
    <div class="details">
      <h3>
        <slot name="heading" />
      </h3>
      <slot />
    </div>
  </div>
</template>

<style scoped>
.item {
  @apply flex mt-8;
}

.details {
  @apply flex-1 text-sm ml-4;
}

i {
  @apply w-8 h-8 flex place-items-center place-content-center text-gray-800;
}

h3 {
  @apply text-xl font-medium mb-2 text-gray-800;
}

@media (min-width: 1024px) {
  .item {
    @apply mt-0;
  }

  i {
    @apply w-12 h-12 border border-gray-300 rounded-lg;
  }
}
</style>
