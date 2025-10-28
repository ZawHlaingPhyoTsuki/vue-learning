<script setup>
import SlotComponent from "./SlotComponent.vue";
import StaticPropsComponent from "./StaticPropsComponent.vue";
const age = 20;
</script>

<template>
  <!-- <StaticPropsComponent name="Zaw" :age="age"/> -->
  <StaticPropsComponent/>
  <SlotComponent>
    <h1>Content1</h1>
    <h1>Content2</h1>
  </SlotComponent>
</template>
