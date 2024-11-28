<template>
    <div class="container">
      <div class="row">
        <div 
          v-for="(joke, index) in jokes" 
          :key="index" 
          class="col-12 col-md-6 col-lg-4 d-flex justify-content-center">
          <chuck-card :iconUrl="joke.icon_url" :value="joke.value" />
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import ChuckCard from './components/ChuckCard.vue';
  
  export default {
    name: 'App',
    components: {
      ChuckCard
    },
    data() {
      return {
        jokes: [
          {
            icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
            value: "Chuck Norris can skydive into outer space."
          },
          {
            icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
            value: "The chief export of Chuck Norris is pain."
          },
          {
            icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
            value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants."
          },
          {
            icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
            value: "Time waits for no man. Unless that man is Chuck Norris."
          },
          {
            icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
            value: "If you spell Chuck Norris in Scrabble, you win. Forever."
          }
        ]
      };
    }
  };
  </script>
  
  <style>
  .container {
    margin-top: 2rem;
  }
  </style>
  