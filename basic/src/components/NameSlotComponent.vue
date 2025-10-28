<script setup></script>

<template>
    <div class="card">
      <div><slot name="name"></slot></div>
      <div><slot name="age"></slot></div>
    </div>
</template>

<style scoped>
.card {
  border: 1px solid #ccc;
  padding: 1rem;
  border-radius: 8px;
  display: flex;
  flex-direction: column;
}
</style>
