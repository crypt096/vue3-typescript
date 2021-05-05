<template>
  <div class="app">{{ name }} - {{ age }}</div>
  <button @click="changeName('Zelda')">Change name</button>
  <button @click="changeAge(55)">Change age</button>
</template>

<script lang="ts">
import { defineComponent, reactive } from "vue";

export default defineComponent({
  name: "App",
  components: {},
  setup() {
    const state = reactive({
      name: "Link",
      age: 25 as string | number,
    });
  },
  methods: {},
});
</script>

<style>
</style>
 