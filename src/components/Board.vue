<template>
  <div id="board">
    <div>
      <Box v-for="box in boxes" :key="box" :class="{brown: box % 3}"></Box>
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
  data() {
    return {
      boxes: 57,
    };
  },
};
</script>

<style scoped>
#board {
  /* width: 400px;
  height: 400px; */
  background-color: lightblue;
}
.brown {
  border-color: brown;
}
</style>
