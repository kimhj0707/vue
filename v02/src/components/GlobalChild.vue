<template>
  <h1>전역 컴포넌트</h1>
  <p>전역 컴포넌트 입니다.</p>
</template>

<script>
export default {
  beforeCreate() {
    console.log("GlobalComponent beforeCreate");
  },
  created() {
    console.log("GlobalComponent created");
  },
  beforeMount() {
    console.log("GlobalComponent beforeMount");
  },
  mounted() {
    console.log("GlobalComponent mounted");
  },
  beforeUpdate() {
    console.log("GlobalComponent beforeUpdate");
  },
  updated() {
    console.log("GlobalComponent updated");
  },
  deforeUnmount() {
    console.log("GlobalComponent deforeUnmount");
  },
  unmounted() {
    console.log("GlobalComponent unmounted");
  },
};
</script>

<style scoped>
h1 {
  color: red;
}
p {
  color: orangered;
}
</style>
