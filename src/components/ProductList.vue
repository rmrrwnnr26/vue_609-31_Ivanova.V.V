<script setup>
import VProduct from "./VProduct.vue";
defineProps({
    items: Array,
});
</script>
<template>
  <div class="grid grid-cols-5 gap-5">
    <v-product
        v-for="item in items"
        :key="item.id"
        :img-url="item.imageUrl"
        :title="item.title"
        :price="item.price.toLocaleString('ru-RU')"
    ></v-product>
  </div>
</template>