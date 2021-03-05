<template>
  <div style="width: 200px;">
    <h1>{{ selected }}</h1>
  </div>
</template>

<script>
export default {
  props: {
    selected: Number,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
