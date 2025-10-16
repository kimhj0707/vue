<script>
export default {
  data() {
    return {
      chk: false,
    };
  },
  computed: {
    yesNo() {
      if (this.chk) {
        return "예";
      } else {
        return "아니오";
      }
    },
  },
};
</script>

<template>
  <input type="checkbox" v-model="chk" />{{ yesNo }} {{ yesNo }} {{ yesNo }}
</template>

<style></style>
