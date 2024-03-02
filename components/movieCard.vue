<script setup>
defineProps(["movieid", "title", "date", "poster"]);
</script>

<template>
  <div class="bg-white rounded-lg shadow-md overflow-hidden m-2 px-1">
    <div
      class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
    >
      <div class="overflow-hidden p-2">
        <img
          class="h-400 w-300 object-cover"
          :src="`https://image.tmdb.org/t/p/w300/` + poster"
          alt="Placeholder Image"
        />
      </div>
      <div class="p-1">
        <a href="#">
          <h5
            class="mb-1 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
          >
            {{ title }}
          </h5>
        </a>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
          Release Date: {{ date }}
        </p>
        <div class="mt-3 p-2 text-right">
          <NuxtLink
            :to="`movie/${movieid}`"
            class="bg-rose-500 hover:bg-rose-600 text-white font-medium py-2 px-4 rounded"
            >Get Details</NuxtLink
          >
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.h-400 {
  height: 400px;
}
.w-300 {
  width: 300px;
}
</style>
