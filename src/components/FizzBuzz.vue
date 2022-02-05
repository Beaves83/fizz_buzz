<template>
  <div class="fizzBuzz">
    <h1>{{ welcomeMessage }}</h1>
    <p>
      In this game you could see the functionality of Fizz Buzz for numbers 1 to 100.
    </p>
    <button class="btn btn-primary text-white"
    @click="executeGame">Ready Player One!</button>
    <div class="card card-body mt-5" style="width: 50rem;">
      <p class="card-text pb-5 text-justify">{{(solution.length > 0) ? solution : ''}}</p>
    </div>
     <button v-if="solution.length>0" class="btn btn-danger text-white btn-sm "
    @click="cleanSolution">Reset</button>
  </div>
</template>

<script>
export default {
  name: 'FizzBuzz',
  props: {
    welcomeMessage: String,
  },
  data() {
    return {
      solution: [],
    };
  },
  methods: {
    executeGame() {
      this.cleanSolution();
      for (let i = 1; i <= 100; i += 1) {
        if ((i % 3 === 0) && (i % 5 === 0)) {
          this.solution.push('Fizz Buzz');
        } else if (i % 3 === 0) {
          this.solution.push('Fizz');
        } else if (i % 5 === 0) {
          this.solution.push('Buzz');
        } else {
          this.solution.push(i);
        }
      }
    },
    cleanSolution() {
      this.solution.splice(0, this.solution.length);
    },
  },
};
</script>

<style lang="scss">
.card {
    margin: 0 auto;
    float: none;
    margin-bottom: 10px;
  }
</style>
