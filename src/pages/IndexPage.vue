<template>
  <div
    :class="[
      'py-8 p-4 sm:px-16 max-w-6xl mx-auto flex flex-col gap-4 midjourney justify-center overflow-y-auto items-center',
    ]"
  >
    <h2 :class="['mt-4', 'text-center', 'text-2xl']">
      MidJourney Prompt Helper
    </h2>

    <div
      :class="['w-full text-black rounded-2xl text-2xl flex justify-between']"
    >
      <q-input
        type="textarea"
        v-model="mainIdeaText"
        autofocus
        counter
        @keyup.enter.stop
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const mainIdeaText = ref<string>('');
</script>
