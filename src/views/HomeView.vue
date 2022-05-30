<script setup lang="ts">
import Navbar from '@/components/NavbarWrapper.vue';
import UserCard from '@/components/UserCard.vue';
import { useTitle } from '@vueuse/core';

useTitle('Home');
</script>

<template>
  <Navbar>
    <main class="centered w-[95%] md:w-9/12">
      <UserCard />
    </main>
  </Navbar>
</template>

<style scoped>
.centered {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
