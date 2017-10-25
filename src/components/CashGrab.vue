<template>
  <div>
    <h1>{{ hook }}</h1>
    <h2>{{ line }}</h2>
    <p>{{ sinker }}</p>
    <button class="button" @click="sendTo">CLICK HERE YOU LUCKY DOG!!!</button>
  </div>
</template>

<script>
  export default {
    name: 'CashGrab',
    data () {
      return {
        hook: 'Congratulation!',
        line: 'You are wiener!!!',
        sinker: 'You are selected to be one in million million lucky wiener of Grand Prize of 100,000,000 dollars! Click Below to Claim!!!',
        bait: 'https://www.youtube.com/watch?v=hpj6Nuc1SI4'
      }
    },
    methods: {
      sendTo () {
        window.location.href = this.bait
      }
    }
  }
</script>

<style scoped>
  body {
    position: relative;
  }
  h1 {
    animation: annoying-blink linear 0.5s infinite;
  }

  .button {
    font-size: 5rem;
    background-color: #22AA00;
    color: #FFF;
    padding: 5rem;
    position: relative;
    animation: scroll-button linear 2.5s infinite;
    cursor: pointer;
  }

  @keyframes annoying-blink {
    0% {
      color: #FF0000;
    }
    50% {
      color: #00FF00;
    }
    100% {
      color: #FF0000;
    }
  }

  @keyframes scroll-button {
    0% {left: 0px;}
    10% {left: 100em;}
    11% {left: -100em;}
    25% {left: 0em;}
  }
</style>
