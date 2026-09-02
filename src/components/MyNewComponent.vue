<script setup>
import { ref } from "vue";
const count = ref(0);
function increment() {
    count.value++;
}
</script>

<template>
    <h1>Composition API</h1>
    <h2>{{ count }}</h2>
    <button @click="increment">+</button>
</template>