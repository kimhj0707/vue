<template>
  <button class="fancy-btn">
    <slot :buttonname>디폴트 문자</slot>
  </button>
</template>

<script>
export default {
  data() {
    return {
      buttonname: "잘가!!!!!",
    };
  },
};
</script>
