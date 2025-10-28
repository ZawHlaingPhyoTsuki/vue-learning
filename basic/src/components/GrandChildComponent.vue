<template>
  <h4>Grand Child</h4>
  <p>Inject username: {{ username }}</p>
</template>

<script setup>
import { inject } from "vue";

const username = inject("username");
</script>
