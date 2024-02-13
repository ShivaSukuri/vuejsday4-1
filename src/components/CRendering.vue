<template>
<div class="main">
    <h1>Conditional Rendering</h1>
    <hr>
    <h1>v-if</h1>
    <p>Only if the condition is true it will render</p>

    <div v-if="isFound">
        <h1>Hii iam Shiva</h1>
    </div>
    <div v-else><h1>iam not Shiva</h1></div>
    <button @click="change">submit</button>
</div>

</template>


<script setup lang="ts">
import {ref} from "vue";

const isFound=ref(false);
const change=()=>{
    isFound.value =! isFound.value  ;
}

</script>


<style>
div{
    display:flex;
    flex-direction:column;
}
</style>
