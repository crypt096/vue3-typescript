<template>
  <div class="app">{{ name }} - {{ age }}</div>
  <button @click="changeName('Zelda')">Change name</button>
  <button @click="changeAge(55)">Change age</button>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {},
  data() {
    return {
      name: "Link",
      age: 25 as number | string,
    };
  },
  methods: {
    changeName(newName: string) {
      this.name = newName;
      return newName;
    },
    changeAge(newAge: number | string) {
      this.age = newAge;
      return newAge;
    },
  },
});
</script>

<style>
</style>
 