<script setup lang="ts">
import { useDark } from '@/composables/useDark';
import Sun from '@/assets/icons/SunIcon.vue';
import Moon from '@/assets/icons/MoonIcon.vue';
import Logo from '@/assets/icons/staaphLogo.vue';

const { userTheme, toggleTheme } = useDark();
</script>

<template>
  <main>
    <nav class="p-5 border-b border-gray-500 flex justify-between">
      <router-link to="/"><Logo /></router-link>
      <button>
        <Sun @click="toggleTheme" v-if="userTheme === 'dark'" class="w-8 h-8" />
        <Moon v-else @click="toggleTheme" class="w-8 h-8" />
      </button>
    </nav>
    <slot></slot>
  </main>
</template>
