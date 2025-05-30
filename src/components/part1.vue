<template>
  

<h1>{{ number }}</h1>

<button @click="plus">ADD</button>
<button @click="minus">Minus</button>

</template>

<script setup>
import {ref} from "vue";
let number =ref(900);
const plus =()=>{
number.value= number.value +1;
console.log(number);
}
const minus =()=>{

number.value = number.value -1;
console.log(number);
}

</script>
