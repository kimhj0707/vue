<template>
  <h1>App.Vue</h1>
  <h1>Count : {{ cnt }}</h1>
  <GlobalChild v-if="cnt == 2" />
  <button @click="counter">Count + 1</button>
  <button @click="discounter">Count - 1</button>
</template>

<script>
import GlobalChild from "./components/GlobalChild.vue";

export default {
  data() {
    return {
      cnt: 1,
    };
  },
  beforeCreate() {
    console.log("beforeCreate");
  },
  created() {
    console.log("created");
  },
  beforeMount() {
    console.log("beforeMount");
  },
  mounted() {
    console.log("mounted");
  },
  beforeUpdate() {
    console.log("beforeUpdate");
  },
  updated() {
    console.log("updated");
  },
  deforeUnmount() {
    console.log("deforeUnmount");
  },
  unmounted() {
    console.log("unmounted");
  },
  methods: {
    counter() {
      this.cnt++;
    },
    discounter() {
      this.cnt--;
    },
  },
};
</script>
<style lang="scss" scoped></style>
