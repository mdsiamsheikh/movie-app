<script setup></script>

<template>
  <div class="flex flex-col md:flex-row">
    <div class="md:w-1/2 p-8">
      <img
        src="https://cdn.pixabay.com/photo/2015/11/03/08/58/meeting-1019875_960_720.jpg"
        alt="Contact Us"
      />
    </div>
    <div class="md:w-1/2 p-8 shadow-md">
      <form>
        <label for="name" class="block text-lg font-bold mb-2">Name</label>
        <input
          type="text"
          id="name"
          name="name"
          class="w-full border border-gray-300 p-2 mb-4 rounded-lg"
        />
        <label for="email" class="block text-lg font-bold mb-2">Email</label>
        <input
          type="email"
          id="email"
          name="email"
          class="w-full border border-gray-300 p-2 mb-4 rounded-lg"
        />
        <label for="message" class="block text-lg font-bold mb-2"
          >Message</label
        >
        <textarea
          id="message"
          name="message"
          class="w-full border border-gray-300 p-2 mb-4 rounded-lg"
        ></textarea>
        <button
          type="submit"
          class="bg-rose-500 hover:bg-rose-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
        >
          Submit
        </button>
      </form>
    </div>
  </div>
</template>
