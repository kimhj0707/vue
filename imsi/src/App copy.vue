<template>
  <h1 :class="titleClass">나를 빨갛게 만들어 보세요.</h1>
  <button @click="good1">클릭</button>
</template>

<script setup>
import { ref } from "vue";

const titleClass = ref("");

const good1 = () => {
  titleClass.value = "title";
};

function good() {
  titleClass.value = "title";
}
</script>

<style scoped>
.title {
  color: red;
}
</style>
