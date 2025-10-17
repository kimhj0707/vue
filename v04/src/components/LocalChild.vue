<template>
  <div>
    나는 Child component 입니다. ({{ c }})
    <input type="text" ref="myInput" v-model="c" />
    <button @click="emitToParent">부모 이벤트 호출</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      c: 5,
    };
  },
  methods: {
    emitToParent() {
      this.$emit("createPost", this.c);
    },
  },
};
</script>
