<script setup>
import { ref } from "vue";
import Content1 from "./Content1.vue";
import Content2 from "./Content2.vue";
import Content3 from "./Content3.vue";

const currentTab = ref("Content1");

const tabs = {
  Content1,
  Content2,
  Content3,
};
</script>

<template>
  <button @click="currentTab = 'Content1'">Tab 1</button>
  <button @click="currentTab = 'Content2'">Tab 2</button>
  <button @click="currentTab = 'Content3'">Tab 3</button>

  <component :is="tabs[currentTab]"></component>
</template>
