<template>
    <div class="pb-4" v-if="showMessage">
        <button type="button" class="btn btn-lg btn-danger" @click="showAlert">
        You discovered the Easter Egg!</button>
    </div>
</template>
<script>

export default {
  name: 'EasterEgg',
  props: {
    counter: {
      type: Number,
      default: 0,
    },
  },
  computed: {
    showMessage() {
      return (this.counter > 2);
    },
  },
  methods: {
    showAlert() {
      // eslint-disable-next-line no-alert
      alert('This project was developed by Bibi Ruiz');
    },
  },
};
</script>
