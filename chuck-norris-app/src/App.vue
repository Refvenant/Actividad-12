<template>
   <div id="app">
    <h1>Chuck Norris Facts</h1>
    <ul>
      <li v-for="(fact, index) in chuckFacts" :key="index" class="fact">
        {{ fact.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      chuckFacts: [
        { value: "Chuck Norris can skydive into outer space." },
        { value: "The chief export of Chuck Norris is pain." },
        { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { value: "Time waits for no man. Unless that man is Chuck Norris." },
        { value: "If you spell Chuck Norris in Scrabble, you win. Forever." }
      ]
    };
  }
};
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  text-align: center;
  margin-top: 50px;
}

.fact {
  margin-bottom: 20px;
  padding: 10px;
  background-color: #f0f0f0;
  border-radius: 5px;
}
</style>
