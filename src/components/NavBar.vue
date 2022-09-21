<script setup>
  import { ref } from 'vue'
  const brand = ref('🏛️ Agency Records')
</script>

<template>
  <nav>
    <div class="Wrapper">
      <RouterLink :to="{ name: 'Home' }" class="brand">
        <span class="brand-title">{{ brand }}</span>
      </RouterLink>
      <div class="menu">
        <a href="#" class="menu-item">Departments</a>
        <a href="#" class="menu-item">Settings</a>
        <a href="#" class="menu-login">Logout</a>
      </div>
    </div>
  </nav>
</template>

<style scoped lang="postcss">
  nav {
    @apply flex h-20  bg-yellow-900 text-rose-100;
    .Wrapper {
      @apply container mx-auto  flex w-full  items-center justify-between;
      .brand {
        &-title {
          @apply text-3xl font-semibold text-red-300;
        }
      }
      .menu {
        @apply flex gap-4;
        &-item {
          @apply rounded-2xl px-3 py-3 hover:bg-blue-700 hover:text-red-300;
        }
        &-login {
          @apply rounded-2xl bg-red-600 px-3 py-3 text-rose-100 hover:bg-slate-500;
        }
      }
    }
  }
</style>
