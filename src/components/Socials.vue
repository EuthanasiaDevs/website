<script lang="ts">
  import { defineComponent } from 'vue'

  export default defineComponent({
    setup() {
      const socials = [
        {
          label: 'Github',
          icon: 'fab fa-github',
          url: 'https://github.com/EuthanasiaDevs/',
        },
        {
          label: 'Instagram',
          icon: 'fab fa-instagram',
          url: 'https://www.instagram.com/euthanasiacommunity/',
        },
        {
          label: 'Discord',
          icon: 'fab fa-discord',
          url: 'https://discord.gg/euthanasia',
        },
        {
          label: 'FiveM',
          icon: 'fas fa-server',
          url: 'fivem://connect/euthanasia-community.com',
        },
      ]

      return { socials }
    },
  })
</script>
<template>
  <div class="fixed bottom-0 w-10 left-10">
    <ul class="flex flex-col items-center p-0 m-0 list-none line">
      <li v-for="social in socials" :key="social.url" class="mb-5">
        <a
          :href="social.url"
          target="_blank"
          rel="nofollow noopener noreferrer"
          :aria-label="social.label"
        >
          <i :class="social.icon" />
        </a>
      </li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>
  .line {
    &::after {
      content: '';
      display: block;
      width: 1px;
      height: 2rem;
      margin: 0 auto;

      @apply dark:bg-white bg-black;
    }
  }
</style>
