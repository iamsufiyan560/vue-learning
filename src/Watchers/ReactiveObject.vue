<script setup>
import { reactive, watch } from "vue";
const state = reactive({ username: "alex" });

watch(state, (newVal, oldVal) => {
  console.log("new value", newVal);
  console.log("old value", oldVal);
});
</script>

<template>
  <h1>{{ state.username }}</h1>
  <button @click="state.username = 'jordan'">Change Name</button>
</template>
