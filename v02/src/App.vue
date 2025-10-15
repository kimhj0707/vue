<script>
export default {
  data() {
    return {
      kValue: "",
    };
  },
  methods: {
    getKey(e) {
      // this.kValue = e.key;
      alert("alt - s 를 누르셨네요");
    },
  },
};
</script>

<template>
  <input type="text" v-on:keydown.alt.s="getKey" /><br />
  <span>{{ kValue }}</span>
</template>

<style></style>

.enter .tab .delete .esc .space .up .down .left .right .center
