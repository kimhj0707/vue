<template>
  <h1>나는 부모</h1>
  <button @click="ageInc">age ++</button>
  <ChildCom v-bind:name="name" v-bind:age="age" />
</template>

<script>
import ChildCom from "./components/ChildComponent.vue";
export default {
  data() {
    return {
      name: "Khj",
      age: 35,
    };
  },
  components: {
    ChildCom,
  },
  methods: {
    ageInc() {
      this.age++;
    },
  },
};
</script>

<style></style>
