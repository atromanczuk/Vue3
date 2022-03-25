<template>
  <div>
    <div>{{ text }}</div>
    <div>{{ algo }}</div>
  </div>
</template>

<script>
import base from "@/minixins/base";

export default {
  name: "App",
  mixins: [base],
  data() {
    return {
      text: "Hola Vue",
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

/*desaparece*/
.fade-leave-to,
.fade-enter-from {
  opacity: 0;
}

/*aparece*/
.fade-leave-active,
.fade-enter-active {
  transition: opacity 0.5s ease;
}
</style>
