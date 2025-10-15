<script>
export default {
  data() {
    return {
      sports: ["Baseball", "Football", "Volleyball", "Swimming"],
    };
  },
};
</script>

<template>
  <ul>
    <li v-for="(sport, index) in sports">{{ index + 1 }} {{ sport }}</li>
  </ul>
</template>

<style></style>
