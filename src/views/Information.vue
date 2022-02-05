<template>
  <div class="information">
    <img alt="Info" class="pb-5" src="../assets/information.png">
    <div class="card card-body" style="width: 50rem;">
      <h1 class="card-title">This is the information about de game</h1>
      <Instructions />
    </div>
  </div>
</template>
<script>
import Instructions from '@/components/Instructions.vue';

export default {
  name: 'Information',
  components: {
    Instructions,
  },
};
</script>
<style lang="scss">

</style>
