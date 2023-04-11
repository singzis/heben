<script setup lang="ts">
import { ref } from 'vue'
import Main from './components/main.vue'
import Header from './components/header.vue'
import SubFooter from './components/subFooter.vue'
import Footer from './components/footer.vue'
import MenuModal from './components/menuModal.vue'

const menuModal = ref(false)

const toggleMenuModal = () => {
  menuModal.value = !menuModal.value
  document.body.classList.toggle('overflow-hidden')
}
</script>

<template>
  <main class="relative text-zinc-950 h-full bg-[#f2f0ed]">
    <Header :toggleMenuModal="toggleMenuModal" />
    <Main />
    <SubFooter />
    <Footer />
    <slot v-if="menuModal"><MenuModal :toggleMenuModal="toggleMenuModal" /></slot>
  </main>
</template>

<style scoped></style>
