<script>
export default {
  data() {
    return {
      site_name: "Daum",
      url: "https://daum.net",
      src: "https://i.namu.wiki/i/xxyTLDbYnN4uGEFNR-VpNVMa-iK5c5-zvzd4VOoBOuMBfzhqx1K8mcToaQ7K17D7OoqypoJolu3uAKURgooBOQ.webp",
    };
  },
  methods: {
    clickAr: function () {
      this.site_name = "Naver";
      this.url = "https://naver.com";
    },
  },
};
</script>

<template>
  <a :href="url">{{ site_name }}</a>
  <img :src="src" />
  <button @click="clickAr">버튼</button>
</template>

<style></style>
