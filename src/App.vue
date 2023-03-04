<script setup>
import HelloWorld from './components/HelloWorld.vue'
const packages = [
  {
    name:'@cfdi/xml',
    icon: 'xml'
  },
  {
    name:'@cfdi/csd',
    icon: 'csd'
  },
 
]
</script>

<template>
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
<div class="grid grid-cols-4 gap-4">
  <div v-for="(lib,i) of packages"  :key="i" >
    {{lib}}
    <a href="#" :key="i" class="block max-w-sm p-6 bg-white border border-gray-200 rounded-lg shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
      {{lib.name}}
    </h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.</p>
</a>
  </div>
</div>

</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
