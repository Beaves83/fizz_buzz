<template>
  <div class="home">
    <img alt="Fizz Buzz" class="pb-5" src="../assets/videogame.png">
    <FizzBuzz welcome-message="Welcome to Fizz Buzz Game"/>
  </div>
</template>

<script>
// @ is an alias to /src
import FizzBuzz from '@/components/FizzBuzz.vue';

export default {
  name: 'Home',
  components: {
    FizzBuzz,
  },
};
</script>
