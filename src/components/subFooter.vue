<template>
  <div class="sub_footer text-8xl font-black flex justify-center pt-32 pb-32">
    <div class="truncate sub_footer_hover">
      <div
        class="relative flex text-center pl-4 pr-4 cursor-pointer"
        v-for="item in ['TO DO WHAT', 'YOU WANT TO DO']"
      >
        <slot :row="item">
          <span class="inline-block w-full text-transparent text_stroke">
            {{ item }}
          </span>
          <span class="sub_footer__fill">
            <span class="sub_footer__inner">{{ item }}</span>
          </span>
        </slot>
      </div>
    </div>
  </div>
</template>
