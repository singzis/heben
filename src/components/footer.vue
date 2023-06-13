<script setup lang="ts">
import webRouter from '../assets/json/webRouter.json'
const routers = webRouter.webRouter
</script>

<template>
  <div class="bg-black p-20">
    <!-- <ul class="grid grid-cols-3 gap-12 mb-20">
      <li v-for="r in routers" :key="r.name" class="text-center">
        <slot :row="r">
          <a :href="r.path" class="text-3xl text-white hover:text-white">{{
            r.name
          }}</a>
        </slot>
      </li>
    </ul> -->
    <a
      class="text-center text-white hover:text-white w-full"
      href="https://beian.miit.gov.cn/"
      target="_blank"
      >蜀ICP备2023008006号</a
    >
  </div>
</template>
