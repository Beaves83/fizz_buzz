<template>
  <div class="home">
    <EasterEgg/>
    <img alt="Fizz Buzz" class="pb-5" src="../assets/videogame.png">
    <FizzBuzz welcome-message="Welcome to Fizz Buzz Game"/>
  </div>
</template>

<script>
import FizzBuzz from '@/components/FizzBuzz.vue';
import EasterEgg from '@/components/EasterEgg.vue';

export default {
  name: 'Home',
  components: {
    FizzBuzz,
    EasterEgg,
  },

};
</script>
