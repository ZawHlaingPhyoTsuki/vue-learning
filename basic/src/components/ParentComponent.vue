<template>
  <div>
    <h2>Parent</h2>
    <ChildComponent />
  </div>
</template>

<script setup>
import { provide, ref } from "vue";
import ChildComponent from "./ChildComponent.vue";

const username = ref("Zaw Hlaing Phyo");
provide("username", username);

setTimeout(() => {
  username.value = 'New Name!'
}, 2000)
</script>
