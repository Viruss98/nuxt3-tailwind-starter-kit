<script setup>
const langs = ['en', 'vi']

const locale = ref('en')
</script>

<template>
  <select
    v-model="locale"
    class="
      text-white text-xs
      bg-transparent
      uppercase
      border border-skin-base
      rounded
      bg-none
      px-2
      py-1
      focus:ring-0
    "
  >
    <option v-for="(lang, i) in langs" :key="`Lang${i}`" :value="lang">
      {{ lang }}
    </option>
  </select>
</template>
