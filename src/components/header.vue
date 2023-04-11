<script setup lang="ts">
import Menu from './menu.vue'

interface Props {
  toggleMenuModal: () => void
}

const props = withDefaults(defineProps<Props>(), {
  toggleMenuModal: () => {},
})
</script>
<template>
  <section class="h-32 top-0 flex items-center pl-16 pr-16">
    <div class="basis-32">
      <span>H</span>
    </div>
    <div class="grow text-center">
      <span>Directory</span>
    </div>
    <div class="basis-32 flex flex-row-reverse">
      <a @click="props.toggleMenuModal">
        <Menu />
      </a>
    </div>
  </section>
</template>
