<script setup lang="ts">
import NavbarTop from '@/components/NavbarTop.vue';
import UserCard from '@/components/UserCard.vue';
</script>

<template>
  <NavbarTop />
  <main class="centered w-[95%] md:w-9/12">
    <UserCard />
  </main>
</template>

<style scoped>
.centered {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
