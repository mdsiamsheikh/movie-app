<template>
  <section
    class="hero-section bg-cover bg-center"
    style="
      background-image: url(https://img.freepik.com/free-vector/3d-realistic-cinema-film-strip-clapper-board-background_1017-38429.jpg?w=1380&t=st=1728367078~exp=1728367678~hmac=514866d10b3b2b3d895c84368df45f675e8618b2c7253c48235238136cd9a72b);
    "
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
