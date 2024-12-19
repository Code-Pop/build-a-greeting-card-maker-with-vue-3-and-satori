<template>
  <div class="w-full bg-red-500 h-full flex flex-col text-white text-7xl font-bold p-10 items-center justify-center"
    style="background-image: url(/img/sincerely-media-8EhZobADF8M-unsplash.jpg);">
    <div class="font-bold mb-8 " style="font-size: 100px;"> {{ greeting }}</div>
    <img v-if="photo" :src="photo" class="rounded-full border-4 border-red-900 mb-8" style="width:400px;height:400px">
    <div class="bg-red-500 px-2 py-2">From</div>
    <div> {{ name || 'Add your name here' }}</div>
  </div>
</template>

<script setup lang="ts">
defineProps(['name', 'greeting', 'photo'])
</script>
