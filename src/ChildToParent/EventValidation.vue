<script setup>
import { ref } from "vue";
const username = ref("");
const email = ref("");
const password = ref("");
</script>

<template>
  <form @submit.prevent="$emit('userInfo', username, email, password)">
    <input placeholder="name" type="text" v-model="username" />
    <input placeholder="email" type="email" v-model="email" />

    <input placeholder="password" type="password" v-model="password" />
    <button type="submit">Submit</button>
  </form>
</template>
