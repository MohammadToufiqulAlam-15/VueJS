// What is Form Input Binding & How to Bind
// How v-model directive is used?

<template>
  <h1> Vue JS Form </h1>
  <input v-model="firstName" type="text" placeholder="First Name">
  {{ firstName }}
</template>

<script setup >

import {ref} from "vue";
const firstName =ref("");



</script>