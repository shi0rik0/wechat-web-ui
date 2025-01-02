<script setup lang="ts">
import ChatBubble from '@/components/ChatBubble.vue'
</script>

<template>
  <div class="top-bar flex justify-between items-center fixed top-0 left-0 right-0 h-16 z-50">
    <div class="ml-6">
      <img src="@/assets/back.svg" />
    </div>
    <div>
      <span>相亲相爱一家人（5）</span>
    </div>
    <div class="mr-6">
      <img src="@/assets/account.svg" />
    </div>
  </div>
  <div class="flex flex-col h-screen">
    <div class="main-content flex-1 overflow-y-scroll hide-scrollbar">
      <div class="h-16"></div>
      <div>
        <ChatBubble avatar="https://wechat.xbox.work/logo.jpg">123</ChatBubble>
        <ChatBubble avatar="https://wechat.xbox.work/logo.jpg" right>123</ChatBubble>
      </div>
    </div>
    <div class="bottom-bar flex items-center h-16">
      <img src="@/assets/speak.svg" class="mx-2" />
      <input type="text"
        class="flex-1 m-0 w-full h-9 px-2 rounded bg-white outline-none border-0 shadow-none caret-green-500 text-base font-normal" />
      <img src="@/assets/emoji.svg" class="ml-2" />
      <img src="@/assets/extra.svg" class="mx-2" />
    </div>
  </div>
</template>

<style scoped>
.top-bar {
  background-color: rgba(237, 237, 237, 0.8);
  border-bottom: 1px solid rgb(220, 223, 213);
}

.main-content {
  background-color: rgba(237, 237, 237);
}

.bottom-bar {
  background-color: rgba(237, 237, 237);
  border-top: 1px solid rgb(220, 223, 213);
}
</style>
