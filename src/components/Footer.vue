<script setup lang="ts">
  const date = `2019-${new Date().getFullYear()}`
</script>

<template>
  <div class="flex w-full h-16 px-4 py-4 mb-6 md:mb-0">
    <p class="mx-auto footer">© <a href="/">EUTHANASIA</a> {{ date }}</p>
  </div>
</template>

<style lang="scss" scoped>
  .footer {
    font-family: 'Dosis', sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    text-align: center;
    text-transform: uppercase;
    letter-spacing: 0.25em;

    @apply dark:text-white text-black;
    margin: 0 auto;
    -webkit-font-smoothing: antialiased;
  }
</style>
