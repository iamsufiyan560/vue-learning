<script setup>
import EventValidation from "./ChildToParent/EventValidation.vue";
import { ref } from "vue";

// let count = ref(0);
// const increment = () => count.value++;

// import DynamicPropsComponent from "./props/DynamicPropsComponent.vue";
// import StaticPropsComponent from "./props/StaticPropsComponent.vue";
// import PropValidation from "./props/PropValidation.vue";
// import ComplexProps from "./props/ComplexProps.vue";
// import CustomValidator from "./props/CustomValidator.vue";
// const NAME = ref("xyz");
// const LNAME = ref("abc");

// const emit = defineEmits({
//   userInfo: ({ username, email, password }) => {
//     if (!username) {
//       console.log("Please enter your name");
//     }
//     if (!email) {
//       console.log("Please enter your email");
//     }
//     if (!password) {
//       console.log("Please enter your password");
//     } else {
//       return true;
//     }
//   },
// });

// const formHandler = (username, email, password) => {
//   emit("userInfo", { username, email, password });
//   console.log("username: ", username);
//   console.log("email: ", email);
//   console.log("password: ", password);
// };
</script>

<template>
  <!-- <StaticPropsComponent name="book" />
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
  <CustomValidator name="sufiyan" :age="20" password="hjvbvbvbc" /> -->
  <!-- <h1>{{ count }}</h1> -->
  <!-- <ComponentEvent @incrementCount="count++" /> -->
  <!-- <ComponentEvent @incrementCount="increment" /> -->
  <!-- <EventValidation @userInfo="formHandler" /> -->
  <div></div>
</template>

<style scoped></style>
