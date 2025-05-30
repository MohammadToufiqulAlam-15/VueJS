<template>

<h1>{{ products }}</h1>
</template>



<script setup>
import {ref} from "vue";

const products = ref([])

CallAPI();
async function CallAPI(){
  const response = await fetch("https://dummyjson.com/products");
  const data = await response.json();
  console.log(data);
  products.value = data['products'];
}

</script>
