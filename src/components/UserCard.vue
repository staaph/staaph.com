<script setup lang="ts">
import IconBar from '@/components/IconBar.vue';
import GithubIcon from '@/assets/icons/GithubIcon.vue';
import ArrowRight from '@/assets/icons/ArrowRight.vue';
import DiscordIcon from '@/assets/icons/DiscordIcon.vue';
</script>

<template>
  <main
    class="dark:bg-slate-700 bg-slate-300 rounded-lg flex flex-col items-center p-5 sm:p-8 sm:py-12 shadow-lg shadow-gray-900"
  >
    <div class="flex flex-col items-center gap-y-4">
      <section class="flex w-full items-center justify-between">
        <div class="flex flex-col gap-y-4">
          <router-link
            to="/contact"
            class="flex flex-row items-center sm:gap-x-2 hover:opacity-75"
            >Leave me a message
            <ArrowRight class="w-5 h-5" />
          </router-link>
          <div class="flex flex-row gap-x-3 items-center">
            <a
              href="https://github.com/staaph"
              target="_blank"
              rel="noopener noreferrer nofollow"
            >
              <GithubIcon class="w-7 h-7 hover:opacity-75" />
            </a>
            <a
              href="https://discord.com/users/805916788369784882"
              target="_blank"
              rel="noopener noreferrer nofollow"
            >
              <DiscordIcon class="w-7 h-7 hover:opacity-75 cursor-pointer" />
            </a>
          </div>
        </div>
        <img src="@/assets/icons/avatar.png" class="w-28 rounded-full" />
      </section>
      <section class="gap-y-2 flex flex-col">
        <p class="font-medium">Languages & Tools</p>
        <IconBar />
      </section>
    </div>
  </main>
</template>
