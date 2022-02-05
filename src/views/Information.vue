<template>
  <div class="information">
    <EasterEgg :counter="counter" />
    <img alt="Info" class="pb-5" src="../assets/information.png" @dblclick="upCounter">
    <div class="card card-body" style="width: 50rem;">
      <h1 class="card-title">This is the information about de game</h1>
      <Instructions />
    </div>
  </div>
</template>
<script>
import Instructions from '@/components/Instructions.vue';
import EasterEgg from '@/components/EasterEgg.vue';

export default {
  name: 'Information',
  components: {
    Instructions,
    EasterEgg,
  },
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    upCounter() {
      this.counter += 1;
    },
  },
};
</script>
<style lang="scss">

</style>
