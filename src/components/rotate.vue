<script setup lang="ts"></script>
<template>
  <div class="relative w-8 h-8">
    <a
      class="cursor-pointer absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 transition-transform duration-300 hover:-translate-x-1/2 hover:-translate-y-1/2 hover:rotate-[180deg]"
    >
      <slot />
    </a>
  </div>
</template>
