<template>
    <div class="chuck-jokes">
      <h1>Chuck Norris Jokes</h1>
      <ul>
        <li v-for="(joke, index) in jokes" :key="index" class="joke-item">
          {{ joke.value }}
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        jokes: [
          { value: "Chuck Norris can skydive into outer space." },
          { value: "The chief export of Chuck Norris is pain." },
          { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
          { value: "Time waits for no man. Unless that man is Chuck Norris." },
          { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .chuck-jokes {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    padding: 20px;
    text-align: center;
  }
  
  h1 {
    color: #333;
  }
  
  ul {
    list-style-type: none;
    padding: 0;
  }
  
  .joke-item {
    background-color: #fff;
    margin: 10px 0;
    padding: 15px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    font-size: 16px;
    color: #555;
  }
  
  .joke-item:hover {
    background-color: #e7f7ff;
    cursor: pointer;
  }
  </style>
  