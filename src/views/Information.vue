<template>
  <div class="information">
    <img alt="Info image" src="../assets/information.png">
    <h1>This is the information about de game</h1>
    <Instructions />
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
