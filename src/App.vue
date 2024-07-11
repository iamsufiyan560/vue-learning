<script setup>
import { ref } from "vue";
import DynamicPropsComponent from "./props/DynamicPropsComponent.vue";
import StaticPropsComponent from "./props/StaticPropsComponent.vue";
import PropValidation from "./props/PropValidation.vue";
import ComplexProps from "./props/ComplexProps.vue";
import CustomValidator from "./props/CustomValidator.vue";
const NAME = ref("xyz");
const LNAME = ref("abc");
</script>

<template>
  <StaticPropsComponent name="book" />
  <hr />
  <DynamicPropsComponent :firstName="NAME" :lastName="LNAME" />
  <hr />
  <PropValidation fullName="abc xyz pqr" :age="44" />
  <hr />
  <ComplexProps
    :friends="['abc', 'pqr', 'xyz', 'def']"
    :userInfo="{ name: 'ronaldo', age: 20, location: ['Earth', 'MEXICO'] }"
  />
  <hr />
  <CustomValidator name="sufiyan" :age="20" password="hjvbvbvbc" />
</template>

<style scoped></style>
