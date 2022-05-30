<template>
  <main
    class="bg-slate-300 shadow-sm shadow-black border-black border dark:border-none dark:bg-slate-700 rounded-lg px-5 py-3 md:p-5"
  >
    <h1
      class="font-bold text-center mb-4 md:text-xl text-black dark:text-white"
    >
      Contact me
    </h1>
    <form
      action="https://formsubmit.co/9b5363176af611ee5c48952d47dd55a5"
      method="POST"
      class="flex flex-col"
    >
      <!-- E-MAIL -->
      <div class="flex flex-col md:my-2">
        <label
          for="email"
          class="text-black text-xs md:text-base dark:text-white pb-2 font-semibold"
          >E-Mail</label
        >
        <div
          class="flex bg-slate-400 dark:bg-gray-500 outline-none p-2.5 items-center text-black dark:text-white rounded"
        >
          <span><MailIcon class="h-5 w-5" /> </span>

          <input
            type="email"
            name="email"
            class="bg-slate-400 dark:bg-gray-500 outline-none w-full px-2"
            required
          />
        </div>
      </div>
      <!-- SUBJECT -->
      <div class="flex flex-col my-2">
        <label
          for="subject"
          class="text-black dark:text-white pb-2 font-semibold text-xs md:text-base"
          >Subject</label
        >
        <div
          class="flex bg-slate-400 dark:bg-gray-500 outline-none p-2.5 items-center text-black dark:text-white rounded"
        >
          <span>
            <InboxIcon class="h-5 w-5" />
          </span>
          <input
            type="text"
            name="subject"
            class="bg-slate-400 dark:bg-gray-500 outline-none px-2 rounded w-full"
            required
          />
        </div>
      </div>
      <!-- TEXTAREA -->
      <div class="w-full flex flex-col my-2">
        <label
          class="leading-none text-black dark:text-white font-semibold text-xs md:text-base"
          >Message</label
        >
        <textarea
          type="text"
          name="message"
          class="h-32 resize-none leading-none text-black dark:text-white p-3 outline-none mt-4 bg-slate-400 dark:bg-gray-500 rounded"
          required
        ></textarea>
      </div>
      <div class="flex items-center justify-center w-full">
        <button
          class="mt-2 font-semibold leading-none text-white py-4 px-6 bg-blue-700 rounded hover:bg-blue-600 active:scale-90"
        >
          Send message
        </button>
      </div>
    </form>
  </main>
</template>

<script setup lang="ts">
import MailIcon from '@/assets/icons/MailIcon.vue';
import InboxIcon from '../assets/icons/InboxIcon.vue';
</script>
