<script setup lang="ts">
import Main from './components/main.vue'
import Header from './components/header.vue'
import SubFooter from './components/subFooter.vue'
import Footer from './components/footer.vue'
</script>

<template>
  <main class="relative text-zinc-950 h-full bg-[#f2f0ed]">
    <Header />
    <Main />
    <SubFooter />
    <Footer />
  </main>
</template>

<style scoped></style>
