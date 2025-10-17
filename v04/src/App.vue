<template>
  <h1>나는 부모 Component({{ c }})</h1>
  <LocalCom @create-post="callFunction" />
</template>

<script>
import LocalCom from "@/components/LocalChild.vue";
export default {
  data() {
    return {
      c: 0,
    };
  },
  components: {
    LocalCom,
  },
  methods: {
    callFunction(var1) {
      console.log("자식 컴포넌트에서 보낸 이벤트를 수신했어요." + var1);
      this.c = var1;
    },
  },
};
</script>

<style></style>

<!-- aaa bbb ccc -->
<!-- aaa-bbb-ccc 케밥 케이스 -->
<!-- aaa_bbb_ccc 뱀 케이스 -->
<!-- aaaBbbCcc 낙타 -->
<!-- AaaBbbCcc 파스칼 -->
