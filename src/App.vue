<template>

  <div id="app">
    <!-- <img src="./assets/logo.png">
    <HelloWorld/>-->
    <header class="head">
      <h1>Rock Paper Scissors</h1>
    </header>

    <div class="score-board">
      <div id="user-label" class="badge">user</div>
      <div id="computer-label" class="badge">comp</div>
      <span id="user-score">0</span>:
      <span id="comp-score">0</span>
    </div>

    <div class="result">
      <p>Paper covers rock. You Win!</p>
    </div>

    <div class="choices">
      <div class="choice" id="r">
        <img src="./assets/rock1.png" width="150px"  alt>
      </div>
      <div class="choice" id="p">
        <img src="./assets/paper1.png" width="150px"  alt>
      </div>
      <div class="choice" id="s">
        <img src="./assets/scissors1.png" width="150px" alt>
      </div>
    </div>
      <p id="action-message">Make your move</p>
  </div>

</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  }
};
</script>

<style>
* {
  background-color: #ffea00;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}

header{
  background-color: #2c3e50;
  padding: 30px;
  
}


header > h1 {
  background-color: #2c3e50;
  color: white;
  text-align: center;
  font-size: 50px;
}

.score-board{
  margin: 20px auto;
  border: 5px solid #2c3e50;
  border-radius:  5px;
  text-align: center;
  width: 200px;
  color: #2c3e50;
  font-weight: bold;
  font-size: 35px;
  padding: 15px 20px;
  position: relative;
}

.badge{
  background-color: #e25840;
  color: white;
  font-size: 20px;
  padding: 2px 10px;
}

#user-label{
  position: absolute;
  top: 25px;
  left: -30px;
}

#computer-label{
  position: absolute;
  top: 25px;
  left: 160px;
}

.result{
  font-weight: bold;
  font-size: 35px;
  color: #2c3e50;
}

.result > p{
  text-align: center;
}

.choices{
  margin: 50px 0;
  text-align: center;
}

.choice{
  width: 200px;
  height: 200px;
  overflow: hidden;
  border: 6px solid #2c3e50;
  border-radius: 50%;
  margin: 0 20px;
  padding: 20px;
  display: inline-block;
}

.choice:hover{
  cursor: pointer;
  background: #e25840;
}

</style>
