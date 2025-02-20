<script setup lang="ts">
import type ResultContainer from '../components/ResultContainer.vue';

// defineProps<{ age: number }>();
</script>

<template>
  <div class="grid lg:grid-cols-2 grid-cols-1 gap-4 p-4 w-full min-h-screen">
    <div class="flex justify-center items-center p-4 text-2xl">
      <!-- <input
        type="number"
        name="deg"
        id="deg"
        class="bg-white border border-slate-300 rounded-full px-8 py-4 mr-4"
      /> -->
      <!-- <label
        class="group flex items-center bg-white border border-slate-300 rounded-full px-8 py-4 mr-4 cursor-text peer-focus:ring-2 peer-focus:ring-blue-500"
      >
        <input
          type="number"
          class="w-full text-right outline-none bg-transparent peer"
          placeholder="45"
        />
        <span class="ml-2 text-slate-700 pointer-events-none">deg</span>
      </label> -->
      <label
        class="group flex items-center bg-white border border-slate-300 rounded-full px-8 py-4 mr-4 cursor-text peer-focus:outline peer-focus:outline-2 peer-focus:outline-blue-500"
      >
        <input
          type="number"
          class="w-full text-right outline-none bg-transparent peer"
          placeholder="45"
        />
        <span class="ml-2 text-slate-700 pointer-events-none">deg</span>
      </label>

      <button class="bg-sky-500 text-white rounded-full px-8 py-4" onclick="">
        Generate
      </button>
    </div>
    <div class="bg-green-500 text-white p-4 text-center">
      <PreviewContainer />
    </div>
    <div class="bg-red-500 text-white p-4 text-center lg:col-span-2 col-span-1">
      <ResultContainer />
    </div>
  </div>
</template>
