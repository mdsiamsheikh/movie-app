<script setup>
definePageMeta({
  layout: "custom",
});

const route = useRoute();

const { data: movie, error } = await useFetch(`/api/movies/${route.params.id}`);
// console.log(movie);

// Fetch Movie Trailer
const { data: video } = await useFetch(
  `/api/movies/trailer/${route.params.id}`
);

const allvideo = toRaw(video.value.results);

const template = computed(() => {
  let trailer = [];
  for (let i = 0; i < allvideo.length; i++) {
    if (allvideo[i].type === "Trailer") {
      trailer.push(allvideo[i]);
    }
  }
  return trailer[0].key;
});
</script>

<template>
  <div>
    <MovieDetail
      :title="movie.title"
      :date="movie.release_date"
      :poster="movie.poster_path"
      :revenue="movie.revenue"
      :overview="movie.overview"
      :trailer="trailer"
    />
  </div>
</template>

<style lang="css" scoped></style>
