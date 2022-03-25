<template>
  <div>{{ text }}</div>
</template>

<script>
export default {
  data() {
    return {
      text: "Hola Vue",
    };
  },
  beforeCreate() {
    console.log("beforeCreate 1", this.$data, this.$el);
  },
  created() {
    console.log("create 2", this.$data, this.$el);
  },
  mounted() {
    console.log("mounted 3", this.$data, this.$el);
  },
};
</script>

<style></style>
