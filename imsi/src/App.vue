<template>
  <h1 :class="[{ red: isRed, black: !isRed }]">나를 빨갛게 만들어 보세요.</h1>

  <button @click="makeRed">빨강</button>
  <button @click="makeBlack">검정</button>
  <button @click="toggleColor">토글</button>
</template>

<script setup>
import { ref } from "vue";

// true면 빨강, false면 검정
const isRed = ref(false);

// 기존 good1과 동일: 빨갛게
const makeRed = () => {
  isRed.value = true;
};

// 요청하신 "function" 버전: 다시 검게(원래색) 만들기
function makeBlack() {
  isRed.value = false;
}

// 참고용: 토글도 추가
function toggleColor() {
  isRed.value = !isRed.value;
}
</script>

<style scoped>
.red {
  color: red;
}
.black {
  color: #111; /* 검정(원래색), 필요시 다른 색상으로 변경 가능 */
}

/* 버튼 보이기 좋게(참고용, 없어도 됨) */
button {
  margin-right: 6px;
}
</style>
