<template>
    <div class="card" style="width: 18rem;">
      <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
      <div class="card-body">
        <p class="card-text">{{ value }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChuckCard',
    props: {
      iconUrl: {
        type: String,
        required: true
      },
      value: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  .card {
    margin: 1rem;
  }
  </style>
  