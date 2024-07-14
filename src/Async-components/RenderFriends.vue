<script setup>
import { ref } from "vue";
const friends = ref(["sufiyan", "abc", "xyz", " pqr"]);
</script>

<template>
  <h3 v-for="(friend, i) in friends" :key="i">
    {{ friend }}
  </h3>
</template>
