<template>
  <div>
    <div :class="dot"></div>
  </div>
</template>

<script>
export default {
  name: "Dot",
  data() {
    return {
      num: 4,
    };
  },
};
</script>

<style scoped>
.dot {
  background-color: red;
  width: 20px;
  height: 20px;
  border-radius: 50%;
}
</style>