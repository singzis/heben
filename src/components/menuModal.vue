<script setup lang="ts">
import { ref } from 'vue'
import Rotate from './rotate.vue'

interface Props {
  toggleMenuModal: () => void
}

const props = withDefaults(defineProps<Props>(), {
  toggleMenuModal: () => {},
})

const menu = ref(new Array(6))
</script>

<template>
  <div class="fixed bg-transparent w-full h-screen inset-0 backdrop-blur-md">
    <div
      class="w-60 bg-black rounded px-5 py-10 fixed top-8 right-10 text-white"
    >
      <a @click="props.toggleMenuModal" class="absolute right-5 top-5">
        <Rotate>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6 18L18 6M6 6l12 12"
            />
          </svg>
        </Rotate>
      </a>
      <ul>
        <li v-for="li in menu">loading...</li>
      </ul>
      <a href="/" class="text-white">go to resume</a>
    </div>
  </div>
</template>
