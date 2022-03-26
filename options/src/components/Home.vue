<template>
  <div>{{ text }} {{ contador }} {{ obj }}</div>
</template>

<script>
import { ref, reactive } from "vue";

export default {
  setup() {
    const text = ref("Holis");
    const contador = ref(0);
    const obj = reactive({ counter: 0 });

    setInterval(() => obj.counter++, 500);

    return {
      text,
      contador,
      obj,
    };
  },
};
</script>

<style></style>
