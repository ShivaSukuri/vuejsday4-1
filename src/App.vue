<script setup lang="ts">
import CRendering from "@/components/CRendering.vue";
import Home from '@/components/Home.vue';
import EventsList from '@/components/EventsList.vue'
import movie from "@/components/movie.vue"
</script>

<template>
<div> <CRendering /></div><br>
 <div> <Home /></div><br>
 <EventsList /><br>
 <movie />
  
</template>

<style scoped>
div{
    display:flex;
    flex-direction:column;
}

</style>
