<script setup>
import { ref } from "vue";
import One from "../Dynamic_Components/One.vue";
import Two from "../Dynamic_Components/Two.vue";
import Three from "../Dynamic_Components/Three.vue";

const currentTab = ref("ComponentOne");

const tabs = {
  ComponentOne: One,
  ComponentTwo: Two,
  ComponentThree: Three,
};
</script>

<template>
  <!-- With Dynamic Component -->
  <button @click="currentTab = 'ComponentOne'">What is HTML</button>
  <button @click="currentTab = 'ComponentTwo'">What is CSS</button>
  <button @click="currentTab = 'ComponentThree'">What is JS</button>

  <component :is="tabs[currentTab]" />
</template>
