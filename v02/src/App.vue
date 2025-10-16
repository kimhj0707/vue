<template>
  <h1>App.Vue</h1>
  <LocalComponent />
  <GlobalChild />
</template>

<script>
import GlobalChild from "./components/GlobalChild.vue";
import LocalComponent from "./components/LocalChild.vue";
export default {
  components: {
    LocalComponent,
  },
};
</script>

<style lang="scss" scoped></style>
