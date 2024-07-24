<script setup>
import AccordionComponent from "./Projects/AccordionComponent.vue";
import Jokes from "./Projects/Jokes.vue";
import FormValidation from "./Projects/FormValidation.vue";
import ProgressSteps from "./Projects/ProgressSteps.vue";

// import LifeCycleHooks from "./components/LifeCycleHooks.vue";

// const showHide = ref(true);
// import { provide } from "vue";
// import Page from "./Provide_And_Inject/Page.vue";

// Using Provide With Array
// provide("friends", ["Alex", "Jordan", "HuXn", "John"]);

// Using Provide With Object
// provide("games", {
//   id: 1,
//   title: "Epic Adventure Game",
//   genre: ["Action", "Adventure", "RPG"],
//   platform: ["PC", "PlayStation", "Xbox", "Nintendo Switch"],
//   releaseDate: "2022-03-15",
//   developer: {
//     name: "Awesome Game Studios",
//     location: "San Francisco, CA",
//     teamSize: 50,
//   },
// });

// Using Provide With Array Of Objects
// provide("moreGames", [
//   {
//     title: "Space Explorer",
//     genre: "Sci-Fi",
//     platform: "PC",
//     releaseDate: "2023-05-20",
//   },
//   {
//     title: "Fantasy Quest",
//     genre: "Fantasy",
//     platform: "PlayStation",
//     releaseDate: "2023-07-10",
//   },
//   {
//     title: "Inception",
//     director: "Christopher Nolan",
//     genre: "Sci-Fi",
//     releaseDate: "2010-07-16",
//   },
//   {
//     title: "The Shawshank Redemption",
//     director: "Frank Darabont",
//     genre: "Drama",
//     releaseDate: "1994-09-23",
//   },
// ]);

// import Students from "./Provide_And_Inject/Students.vue";

// provide("studentName", "ABC");
// provide("studentAge", 20);
// provide("studentLocation", ["india", "delhi"]);

// import EventValidation from "./ChildToParent/EventValidation.vue";
// import { ref } from "vue";
// import SlotComponent from "./Slots/SlotComponent.vue";
// import FallbackContent from "./Slots/FallbackContent.vue";
// import NamedSlot from "./Slots/NamedSlot.vue";

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

  <div>
    <!-- <SlotComponent>
      <h1>Content 1</h1>
      <h2>Content 2</h2>
    </SlotComponent>
    <hr />
    <FallbackContent /> -->
  </div>

  <!-- <NamedSlot>
    <template v-slot:one>
      <h1>This content will go to slot "one"</h1>
    </template> -->

  <!-- Alternative way -->
  <!-- <template #two>
      <h1>This content will go to slot "two"</h1>
    </template>
  </NamedSlot> -->

  <!-- <Students /> -->

  <!-- <Page></Page> -->

  <!-- <LifeCycleHooks v-if="showHide" />
  <button @click="showHide = !showHide">
    {{ showHide ? "hide" : "show" }} main Component
  </button> -->

  <jokes></jokes>
</template>

<style scoped></style>
