<script setup>
defineProps({
  name: {
    type: String,

    // validator: (propValue) => {
    //   return ['sufiyan', 'adnan', 'xyz'].includes(propValue)
    // },
    validator: (propValue) => ["sufiyan", "adnan", "xyz"].includes(propValue),
  },

  age: {
    type: Number,
    validator: (propValue) =>
      propValue >= 18 && propValue <= 30 ? true : false,
  },

  password: {
    type: String,
    validator: (propValue) => propValue.length >= 8 && true,
  },
});
</script>

<template>
  <h1>Name: {{ name }}</h1>
  <h2>Age: {{ age }}</h2>
  <h3>Password: {{ password }}</h3>
</template>
