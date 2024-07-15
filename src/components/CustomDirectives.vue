<script setup>
// const vFormateDiv = {
//   mounted: (el, binding) => {
//     console.log(el)
//     console.log(binding)

//     el.style.fontSize = '4rem'
//     el.style.fontStyle = 'italic'
//     el.style.color = 'teal'
//   }
// }
// ------------------------------------

// ------------------------------------
// const vFormateDiv = {
//   mounted: (el, binding) => {
//     console.log(binding.value)
//     // el.style.fontSize = binding.value + 'px'
//     el.style.fontSize = `${binding.value}rem`
//     el.style.border = `${binding.value}px solid teal`
//   }
// }
// ------------------------------------
// import { ref } from 'vue'
// const initialFontSize = ref(10)

// const vFormateDiv = {
//   updated: (el, binding) => {
//     el.style.fontSize = `${binding.value}px`
//     el.style.border = `${binding.value}px solid teal`
//   }
// }

// ------------------------------------
// Passing Arguments to custom directive
const vFormateDiv = {
  mounted: (e, binding) => {
    console.log(binding.arg);
    switch (binding.arg) {
      case "orange":
        e.style.color = "orange";
        break;
      case "pink":
        e.style.color = "pink";
        break;
      case "purple":
        e.style.color = "purple";
        break;
      case "teal":
        e.style.color = "teal";
        break;
      default:
        e.style.color = "black";
    }
  },
};
// ------------------------------------

// ------------------------------------
// Shorthand for writing all of that.
// const vFormateDiv = (el) => (el.style.fontSize = '4rem')
// ------------------------------------
</script>

<template>
  <!-- ---------------- -->
  <!-- <div v-formate-div>Using simple custom directive</div> -->
  <!-- <div v-formate-div="4">Passing Value To Parameter</div> -->
  <!-- ---------------- -->

  <!-- ---------------- -->
  <!-- <div v-formate-div="initialFontSize">This is some random text</div>
  <button @click="initialFontSize += 2">Increment Font Size</button> -->
  <!-- ---------------- -->

  <!-- ---------------- -->
  <h1 v-formate-div:default>This text will be black</h1>
  <h1 v-formate-div:orange>This text will be orange</h1>
  <h1 v-formate-div:pink>This text will be pink</h1>
  <h1 v-formate-div:purple>This text will be purple</h1>
  <h1 v-formate-div:teal>This text will be teal</h1>
  <!-- ---------------- -->

  <!-- <h1 v-font-size>Using Function Short Hand</h1> -->
</template>
