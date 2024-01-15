<template>
  <section
    class="hero-section bg-cover bg-center"
    style="background-image: url('/banner.webp')"
  >
    <div class="container sm:mx-auto sm:p-32 p-8">
      <h1 class="text-6xl font-bold text-slate-50 mb-4">Movilix</h1>
      <h3 class="text-lg font-bold text-white">
        <p class="text-lg mb-2">
          123 Main Street<br />
          Bogura, Bangladesh 01235
        </p>
        <p class="text-lg mb-2">
          Phone: 01315536640<br />
          Email: mdsiamsheikh6640@gmail.com
        </p>
      </h3>
      <div class="mt-6">
        <NuxtLink
          to="/registration"
          class="bg-indigo-500 hover:bg-indigo-600 text-white rounded-full font-medium py-2 px-4"
        >
          Get Started
        </NuxtLink>
      </div>
    </div>
  </section>
</template>
