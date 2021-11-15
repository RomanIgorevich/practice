<template>
  <div class="flexbox">
    <board id="board-1">
      <card id="card-1" draggable="true">
        <p>1 card</p>
      </card>
       <card id="card-3" draggable="true">
        <p>3 card</p>
      </card>
       <card id="card-4" draggable="true">
        <p>4 card</p>
      </card>
    </board>
    <board id="board-2">
      <card id="card-2" draggable="true">
        <p>2 card</p>
      </card>
    </board>
  </div>
</template>

<script>
import Board from "./components/Board.vue";
import Card from "./components/Card.vue";

export default {
  components: {
    Board,
    Card,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  background: #f3f3f3;
}
.flexbox {
  display: flex;
  justify-content: space-between;
  width: 100%;
  max-width: 768px;
  height: 100vh;
  overflow: hidden;
  margin: 0 auto;
  padding: 16px;
}
.flexbox .board {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 300px;
  background: #313131;
  padding: 16px;
}
.flexbox .board .card {
  padding: 16px 25px;
  background: #f3f3f3;
  cursor: pointer;
  margin-bottom: 16px;
}
</style>
