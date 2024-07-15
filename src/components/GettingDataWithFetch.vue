<script setup>
import { ref } from "vue";
const data = ref(null);

const fetchData = () => {
  fetch("https://jsonplaceholder.typicode.com/todos/1")
    .then((response) => {
      if (!response.ok) {
        throw new Error(`HTTP error! Status: ${response.status}`);
      }

      return response.json();
    })
    .then((responseData) => {
      data.value = responseData;
    })
    .catch((error) => {
      console.error("Error fetching data:", error);
    });
};
</script>

<template>
  <div>
    <h1>(( Using Fetch ))</h1>
    <button @click="fetchData">Fetch Data</button>

    <div>
      <h2>Data from API:</h2>
      <pre>{{ data }}</pre>
    </div>
  </div>
</template>
