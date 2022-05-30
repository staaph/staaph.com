<script setup lang="ts">
import IconBar from '@/components/IconBar.vue';
import GithubIcon from '@/assets/icons/GithubIcon.vue';
import ArrowRight from '@/assets/icons/ArrowRight.vue';
import DiscordIcon from '@/assets/icons/DiscordIcon.vue';
</script>

<template>
  <main
    class="dark:bg-slate-700 bg-slate-300 rounded flex flex-col items-center p-8 shadow-lg shadow-gray-900"
  >
    <div class="flex flex-col items-center gap-y-4">
      <section class="flex w-full items-center">
        <div class="flex flex-col gap-y-4 sm:w-full">
          <router-link
            to="/"
            class="flex flex-row items-center gap-x-2 hover:opacity-75"
            >Leave me a message
            <ArrowRight class="w-7 h-7 sm:w-5 sm:h-5" />
          </router-link>
          <div class="flex flex-row gap-x-3 items-center">
            <a
              href="https://github.com/staaph"
              target="_blank"
              rel="noopener noreferrer nofollow"
            >
              <GithubIcon class="w-7 h-7 hover:opacity-75" />
            </a>
            <DiscordIcon class="w-7 h-7 hover:opacity-75" />
          </div>
        </div>
        <div class="flex w-full justify-end">
          <img src="@/assets/icons/avatar.png" class="w-28 rounded-full" />
        </div>
      </section>
      <section class="gap-y-2 flex flex-col">
        <p class="font-medium">Languages & Tools</p>
        <IconBar />
      </section>
    </div>
  </main>
</template>
