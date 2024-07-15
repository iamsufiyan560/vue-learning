<script setup>
import { useCounter } from "./useCounter";
const counter = useCounter();
</script>

<template>
  <div>
    <p>Count: {{ counter.count }}</p>
    <button @click="counter.increment">Increment</button>
    <button @click="counter.decrement">Decrement</button>
  </div>
</template>
../shared/useCounter
