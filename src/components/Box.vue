<template>
  <div id="box">
    <Dot />
  </div>
</template>

<script>
import Dot from "./Dot";
export default {
  name: "Box",
  data() {
    return {
      num: true,
    };
  },
  components: {
    Dot,
  },
};
</script>

<style scoped>
#box {
  width: 40px;
  height: 40px;
  background-color: yellow;
  border: 1px solid black;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
