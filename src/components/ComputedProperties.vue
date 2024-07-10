<script setup>
import { ref, computed } from "vue";

const number = ref(5);
const sqaureNumber = computed(() => {
  return number.value * number.value;
});

const firstName = ref("SUFIYAN");
const lastName = ref("CHAUDHARI");
const fullName = computed(() => firstName.value + " " + lastName.value);

const counter = ref(0);

const sqaureCounter = computed(() => counter.value ** 2);
const IncreamentCounter = () => {
  counter.value++;
};
</script>

<template>
  <h1>counterNumber: {{ counter }}</h1>
  <h1>counterSqaureNumber:{{ sqaureCounter }}</h1>

  <button @click="IncreamentCounter">Increament Counter</button>
  <h1>fullName: {{ fullName }}</h1>
  <h1>Originl Number: {{ number }}</h1>
  <h1>Squared Number: {{ sqaureNumber }}</h1>
</template>
