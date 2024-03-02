<script setup></script>

<template>
  <nav class="bg-white border-gray-200 dark:bg-gray-900">
    <div
      class="flex flex-wrap justify-between items-center mx-auto max-w-screen-xl p-4"
    >
      <NuxtLink to="/" class="flex items-center space-x-3 rtl:space-x-reverse">
        <img
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRrZ9AKRWSxh4v4fPLk9hgKnYls7wkHMrVDGQ&usqp=CAU"
          class="h-8 w-8"
          alt=""
        />
        <span
          class="rounded-md font-medium text-2xl text-[#011A24] hover:text-cyan-700"
          >Home</span
        >
      </NuxtLink>

      <div class="flex items-center space-x-6 rtl:space-x-reverse">
        <NuxtLink
          to="/contact"
          class="px-2 py-1 rounded-md font-medium text-xl text-[#011A24] hover:text-cyan-700"
          >Contact</NuxtLink
        >
        <NuxtLink
          to="/registration"
          class="px-2 py-1 rounded-md font-medium text-xl text-[#011A24] hover:text-cyan-700"
          >Registration</NuxtLink
        >
        <NuxtLink
          to="/login"
          class="px-2 py-1 rounded-md font-medium text-xl text-[#011A24] hover:text-cyan-700"
          >Login</NuxtLink
        >
      </div>
    </div>
  </nav>
</template>

<style lang="css" scoped></style>
