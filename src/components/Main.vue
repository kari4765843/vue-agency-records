<script setup>
  import MainSearch from './MainSearch.vue'
</script>

<template>
  <div class="Wrapper">
    <MainSearch />
    <h1>Hello There</h1>
  </div>
</template>

<style scoped lang="postcss">
  .wrapper {
    @apply container mx-auto flex flex-col gap-4 py-5;
  }
</style>
