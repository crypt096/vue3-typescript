<template>
  <div class="job" :key="job.id" v-for="job in jobs">{{ job.title }}</div>
</template>

<style scoped>
</style>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    jobs: {
      required: true,
      type: Array,
    },
  },
});
</script>
