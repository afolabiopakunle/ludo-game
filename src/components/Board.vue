<template>
  <div id="board">
    <div>
      <Box />
    </div>
  </div>
</template>

<script>
import Box from "./Box";
export default {
  name: "Board",
  components: {
    Box,
  },
};
</script>

<style scoped>
#board {
  width: 400px;
  height: 400px;
  background-color: lightblue;
}
</style>
