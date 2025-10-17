<template>
  <h1>나는 App.vue</h1>
  <MainLayout>
    <template #header>
      <h1>Header</h1>
    </template>
    <template #contents>
      <h1>contents</h1>
    </template>
    <template #footer>
      <h1>Footer</h1>
    </template>
  </MainLayout>
  <FancyButton>
    <strong>클릭3</strong>
  </FancyButton>
</template>

<script>
import FancyButton from "@/components/FancyButton.vue";
import MainLayout from "./components/MainLayout.vue";
export default {
  components: {
    FancyButton,
    MainLayout,
  },
};
</script>

<style scoped></style>
