<script setup lang="ts">
import Menu from './menu.vue'
</script>
<template>
  <section
    class="h-32 top-0 flex items-center pl-16 pr-16"
  >
    <div class="basis-32">
      <span>H</span>
    </div>
    <div class="grow text-center">
      <span>Directory</span>
    </div>
    <div class="basis-32 flex flex-row-reverse"><Menu /></div>
  </section>
</template>
