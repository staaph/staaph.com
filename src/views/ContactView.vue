<script setup lang="ts">
import Navbar from '@/components/NavbarWrapper.vue';
import ContactForm from '@/components/ContactForm.vue';
import { useTitle } from '@vueuse/core';

useTitle('Contact');
</script>

<template>
  <Navbar>
    <div class="centered w-[95%] md:w-9/12">
      <ContactForm />
    </div>
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
