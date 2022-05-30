<script setup lang="ts">
import { useDark } from '@/composables/useDark';
import Sun from '@/assets/icons/SunIcon.vue';
import Moon from '@/assets/icons/MoonIcon.vue';

const { userTheme, toggleTheme } = useDark();
</script>

<template>
  <nav>
    <button>
      <Sun @click="toggleTheme" v-if="userTheme === 'dark'" />
      <Moon v-else @click="toggleTheme" />
    </button>
  </nav>
</template>
