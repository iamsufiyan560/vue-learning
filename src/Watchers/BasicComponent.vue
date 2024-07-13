<script setup>
import { ref, watch } from "vue";
const message = ref("Hello, Vue!");

const inputText = ref("");

watch(inputText, (newValue, oldValue) => {
  console.log(newValue);
  console.log(oldValue);
  message.value = `You typed: ${newValue}`;
});
</script>

<template>
  <div>
    <h1>{{ message }}</h1>
    <input v-model="inputText" placeholder="Type something..." />
  </div>
</template>
