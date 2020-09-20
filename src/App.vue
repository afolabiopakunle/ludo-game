<template>
  <div id="app">
    <button @click="startGame" v-if="!gameOn">Start Game</button>
    <Board v-if="gameOn" :num="num" />
  </div>
</template>

<script>
import Board from "./components/Board";

export default {
  name: "App",
  components: {
    Board,
  },
  data() {
    return {
      gameOn: false,
      num: true,
    };
  },
  methods: {
    startGame() {
      this.gameOn = true;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  justify-content: center;
}
</style>
