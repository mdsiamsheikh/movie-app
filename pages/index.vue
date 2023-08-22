<script setup>
// secure movie
const searchError = ref(false);
const searchMovie = (searchInput) => {
  console.log("Search Text: ", searchInput);
  if (searchInput === "") {
    searchError.value = true;
  }
  if (searchInput !== "") {
    searchError.value = false;
  }
};

// fetch Movie
const movieid = ref(123);
const title = ref("Batman Brown City");
const date = ref("20-01-2023");
const poster = ref(
  "https://www.themoviedb.org/t/p/w600_and_h900_bestv2/74xTEgt7R36Fpooo50r9T25onhq.jpg"
);
</script>

<template>
  <div>
    <SearchBar @search-movie="searchMovie" :searchError="searchError" />
    <div
      class="grid md:grid-cols-4 sm:grid-cols-1 justify-items-center bg-cyan-50"
    >
      <MovieCard
        :title="title"
        :date="date"
        :poster="poster"
        :movieid="movieid"
      />
    </div>
  </div>
</template>

<style></style>
