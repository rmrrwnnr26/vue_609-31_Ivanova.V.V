<script>
export default {
    data() {
        return {
            count: 0,
        };
    },
    methods: {
        increment() {
            this.count++;
        },
    },
};
</script>
<template>
    <h1>Options API</h1>
    <h2>{{ count }}</h2>
    <button @click="increment">+</button>
</template>

<style></style>