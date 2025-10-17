<template>
  <button class="fancy-btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ["buttonname"],
};
</script>
