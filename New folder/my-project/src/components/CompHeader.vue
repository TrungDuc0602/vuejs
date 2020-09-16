<template>
  <header>
    <h1>{{ titleHeader }}</h1>
  </header>
</template>

<script>
export default {
  name: "comp-header",
  props: {
    titleHeader: String,
    default: "rong",
  },
  data() {
    return {
      text: "Header",
    };
  },
};
</script>

<style>
</style>