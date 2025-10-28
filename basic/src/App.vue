<script setup>
// import { reactive } from "vue";
// const message = "Hello World!";
// const number = 2;
// const add = (a, b) => a + b;

// let initialState = reactive({ count: 0 });

// let initialState1 = reactive({ val: { count: 0 }, user: ["ZZZ", "AAA"] });
// const changeUser = () => {
//   initialState1.user[0] = "edited-1";
//   initialState1.user[1] = "edited-2";
// };
import { ref } from "vue";
import HelloWorld from "./components/HelloWorld.vue";
import ParentComponent from "./components/ParentComponent.vue";
import GettingDataWithFetch from "./components/GettingDataWithFetch.vue";
import MainComponent from "./components/MainComponent.vue";
let count = ref(0);

// let count1 = 0;
// count1++

let people = ref(["AAA", "BBB", "CCC"]);
</script>

<template>
  <div>
    <!-- <div>
    <h1>{{ message }}</h1>
    <h1>{{ number }}</h1>
    <h1>2 + 2 = {{ 2 + 2 }}</h1>
    <h1>Add Two Numbers: {{ add(2, 2) }}</h1>
  </div>
  <div>
    <h1>Count: {{ initialState.count }}</h1>
    <button @click="initialState.count++">Increment</button>
    <button @click="initialState.count--">Decrement</button>
  </div>

  <div>
    <h1>Current Count: {{ initialState1.val.count }}</h1>
    <h2>Users: {{ initialState1.user.join(', ') }}</h2>
    <button @click="initialState1.val.count += 10">Add 10</button>
    <button @click="changeUser">Change User</button>
    <button @click="initialState1.user.push('edited-3')">
      Add One More User
    </button>
  </div> -->
    <!-- <h1>Count: {{ count }}</h1>
    <button @click="count++">Increment</button>
    <button @click="count--">Decrement</button> -->

    <!-- <h1>Count1: {{ count1 }}</h1>
  <button @click="count1++">Increment</button>
  <button @click="count1--">Decrement</button> -->
    <!-- <div>
      <p v-for="(person, index) in people" :key="index">{{ person }}</p>
    </div>
    <HelloWorld />
    <ParentComponent />
    <GettingDataWithFetch /> -->
    <MainComponent />
  </div>
</template>
