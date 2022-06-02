<script setup>
import HeadComp from "./components/template/HeaderComp.vue";
</script>
<template>
  <HeadComp />
  <RouterView />

  <footer id="footer">footer</footer>
</template>

<style>
@import "@/assets/base.css";

#app {
  font-size: 16px;
  height: 100vh;
  width: 100vw;

  font-weight: normal;
}

header,
footer {
  background-color: rgb(59, 59, 127);
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}
main {
  height: 70%;
}
</style>
