<template>
<div >
<h1>V-for</h1><hr>
<h2>Books</h2>
    <ul v-for="book in books">
    <li>{{book}}</li>
    </ul>
</div>

</template>
<script setup>
const books=["Hitler","one at the call center","half GirlFriend","Fight Club"]
</script>
<style>
div{
    display:flex;
    flex-direction:column;
}
</style>