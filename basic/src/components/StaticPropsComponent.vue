<script setup>
// const props = defineProps(["name", "age"]);
// console.log(props);
defineProps({
  name: {
    type: String,
    default: "Guest",
    required: false,
  },
  age: {
    type: Number,
    default: 16,
    required: false,
  },
});
</script>

<template>
  <div>
    <!-- <h1>{{ props.name }}</h1>
    <h2>{{ props.age }}</h2> -->
    <h1>{{ name }}</h1>
    <h2>{{ age }}</h2>
  </div>
</template>
