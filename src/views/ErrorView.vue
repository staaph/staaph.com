<script setup lang="ts">
import Navbar from '@/components/NavbarWrapper.vue';
import { useTitle } from '@vueuse/core';

useTitle('404');
</script>

<template>
  <Navbar>
    <main class="grid centered place-content-center dark:text-white">
      <h1 class="text-3xl font-medium">404 Not found</h1>
      <p>The page you are looking for cannot be found</p>
      <div class="grid place-content-center p-2">
        <button class="bg-gray-200 rounded p-2 text-black mt-8">
          <router-link to="/">Back home</router-link>
        </button>
      </div>
    </main>
  </Navbar>
</template>

<style scoped>
.centered {
  position: fixed;
  top: 55%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
