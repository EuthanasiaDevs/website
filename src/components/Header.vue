<script setup lang="ts">
  import { ref } from 'vue'

  const darkMode = ref(true)

  const toggleDarkMode = () => {
    darkMode.value = !darkMode.value
    document.documentElement.className = darkMode.value ? 'dark' : ''
  }
</script>

<template>
  <div class="flex justify-between w-full h-16 px-4 py-4">
    <div class="h-full cursor-pointer">
      <svg
        v-if="darkMode"
        xmlns="http://www.w3.org/2000/svg"
        class="w-8 h-8 text-white"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        @click="toggleDarkMode"
      >
        <path
          strokeLinecap="round"
          strokeLinejoin="round"
          strokeWidth="{2}"
          d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"
        />
      </svg>
      <svg
        v-else
        xmlns="http://www.w3.org/2000/svg"
        class="w-8 h-8 text-gray-900"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        @click="toggleDarkMode"
      >
        <path
          strokeLinecap="round"
          strokeLinejoin="round"
          strokeWidth="{2}"
          d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"
        />
      </svg>
    </div>
  </div>
</template>
