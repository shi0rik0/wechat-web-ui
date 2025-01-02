<script setup lang="ts">
const { right = false, avatar } = defineProps<{
  right?: boolean,
  avatar: string,
}>()
</script>

<template>
  <div v-if="!right" class="flex items-center w-full h-20">
    <img :src="avatar" class="rounded w-10 h-10 overflow-clip mx-4" />
    <div class="w-2 h-2 bg-white rotate-45 translate-x-[50%]"></div>
    <div class="bg-white rounded h-10 p-2 flex items-center">
      <slot></slot>
    </div>
  </div>
  <div v-else class="flex justify-end items-center w-full h-20">
    <div class="bg-[#a9ea7a] rounded h-10 p-2 flex items-center">
      <slot></slot>
    </div>
    <div class="w-2 h-2 bg-[#a9ea7a] rotate-45 translate-x-[-50%]"></div>
    <img :src="avatar" class="rounded w-10 h-10 overflow-clip mx-4" />
  </div>
</template>

<style scoped></style>
