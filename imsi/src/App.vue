<template>
  <h1 ref="a" id="b">안녕하세요. 김현중 vue 연습입니다.</h1>
  <button @click="good">봐튼</button>
</template>

<script setup>
import { ref } from "vue";

const a = ref(null);

const good = () => {
  // alert(a.value.innerText);
  alert(document.getElementById("b").innerText);
};
</script>

<style lang="scss" scoped></style>
