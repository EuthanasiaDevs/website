<script setup lang="ts">
  import Header from '@/components/Header.vue'
  import Footer from '@/components/Footer.vue'
  import Socials from '@/components/Socials.vue'
</script>

<template>
  <div class="flex flex-col w-screen h-screen dark:bg-black dark:text-white">
    <Header />
    <main class="flex flex-1 w-screen px-10 md:px-2">
      <div class="flex flex-col items-center m-auto">
        <span></span>
        <h1 class="flex items-center gap-2 text-3xl title">EUTHANASIA</h1>
        <span class="subheading"> &middot; ROLEPLAY &middot; </span>
      </div>
    </main>
    <Footer />
    <Socials />
  </div>
</template>

<style lang="scss" scoped>
  .title {
    @apply dark:text-white text-black;
    font-family: 'Oswald', sans-serif;
    font-size: 120px;
    line-height: 1;
    font-style: normal;
    font-weight: 400;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    text-align: center;
    margin: 41px auto 43px auto;
    padding: 0;
  }
  .subheading {
    @apply dark:text-white text-black;
    font-family: 'Dosis', sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    text-align: center;
    text-transform: uppercase;
    letter-spacing: 0.25em;
    margin: 0 auto;
    -webkit-font-smoothing: antialiased;
  }
</style>
