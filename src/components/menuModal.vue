<script setup lang="ts">
interface Props {
  toggleMenuModal: () => void
}

const props = withDefaults(defineProps<Props>(), {
  toggleMenuModal: () => {},
})
</script>

<template>
  <div class="fixed bg-transparent w-full h-screen inset-0 backdrop-blur-md">
    <a @click="props.toggleMenuModal" class="w-4 h-4">x</a>
  </div>
</template>
