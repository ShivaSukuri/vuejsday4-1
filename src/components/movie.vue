<template>
<div class="content">
    <div class="movie" v-for="movie in movies" :key="movie.name">
      <div>
        <img :src="movie.src" alt="Movie Poster">
        <h1>{{ movie.name }}</h1>
      </div>
    </div>
  </div>
</template>
<script setup>
import {ref} from 'vue';

const movies=[
    {name:"Seetha Ramam",src:"https://m.media-amazon.com/images/M/MV5BN2RjZDJhYzUtOTQ5Yy00OWM3LWE5OTctM2Y0YWVmNzAzODllXkEyXkFqcGdeQXVyMTA3MDk2NDg2._V1_.jpg"},
        {name:"Seetha Ramam",src:"https://m.media-amazon.com/images/M/MV5BN2RjZDJhYzUtOTQ5Yy00OWM3LWE5OTctM2Y0YWVmNzAzODllXkEyXkFqcGdeQXVyMTA3MDk2NDg2._V1_.jpg"}

    ]
</script>
<style>
img {
  height: 200px;
  width: 100%;
}

.content {
  display: flex;
  justify-content: space-between;
}

.movie {
  border: 2px solid black;
  width: 300px;
  margin: 10px;
}

</style>