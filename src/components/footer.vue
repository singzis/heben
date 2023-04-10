<script setup lang="ts">
import webRouter from '../assets/json/webRouter.json'
const routers = webRouter.webRouter
</script>

<template>
  <div class="bg-black p-20">
    <ul class="grid grid-cols-3 gap-12 mb-20">
      <li v-for="r in routers" :key="r.name" class="text-center">
        <slot :row="r">
          <a :href="r.path" class="text-3xl text-white hover:text-white">{{
            r.name
          }}</a>
        </slot>
      </li>
    </ul>
    <div class="pt-20 text-center text-white">京ICP备11018762号</div>
  </div>
</template>
