<template>
  <h1>Child Component</h1>
  <p>Name : {{ name }}</p>
  <p>Age : {{ age }}</p>
</template>

<script>
export default {
  props: ["name", "age"],
  created() {
    console.log(this.name);
  },
  methods: {
    propsUpdater() {
      this.age = 30;
    },
  },
};
</script>
