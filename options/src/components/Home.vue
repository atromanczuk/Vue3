<template>
  <div>{{ obj.counter }}</div>
</template>

<script>
import { reactive, watch } from "vue";

export default {
  setup() {
    // const text = ref("Holis");
    // const contador = ref(0);
    const obj = reactive({ counter: 0 });

    setInterval(() => obj.counter++, 500);

    watch(
      () => obj.counter, //de esta manera conoce el valor más reciente
      (valor, anterior) => {
        console.log(valor, anterior);
      }
    );

    return {
      //   text,
      //   contador,
      obj,
    };
  },
};
</script>

<style></style>
