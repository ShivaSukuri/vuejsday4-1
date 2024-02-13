<template>
<h1>v-on</h1>
<button @click="count++">{{count}}</button>
<input type="text" name="" value="" v-on:input="count1++">{{count1}}
<h1>Event Directives</h1>
<h2>once-calles only once</h2>
<button @click.once="createAlert">create</button>


</template>

<script setup>
import {ref} from 'vue'
const count=ref(0);
const count1=ref(0);
const createAlert=()=>{
    alert("only once")
}
</script>

<style>
button{
    width:70px;
}
input{
    width:200px;
}
</style>
