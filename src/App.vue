<template>
  <div class="w-full h-full flex justify-center items-center">
    <div>
      <div class="w-full max-w-2xl p-4 rounded bg-red-400 text-white">
        <div class="border-2 rounded flex flex-col md:flex-row md:items-center md:gap-8 p-4">
          <img src="/assets/santa.svg" alt="" class="max-w-[12em]" />
          <div>
            <h1 class="font-serif text-4xl">Happy Holidays!</h1>
            <div class="mt-4 bg-white text-black p-2 rounded">TO: {{ form.to }}</div>
            <div class="mt-2 bg-white text-black p-2 rounded">FROM: {{ form.from }}</div>
          </div>
        </div>
      </div>

      <div class="flex flex-col mt-2">
        <label>
          TO : <br />
          <input v-model="form.to" type="text" class="border-2 w-full" />
        </label>
        <label>
          FROM : <br />
          <input v-model="form.from" type="text" class="border-2 w-full" />
        </label>
      </div>
    </div>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

const form = reactive({
  to: '',
  from: '',
})
</script>
