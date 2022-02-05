<template>
    <div class="pb-4" v-if="showMessage">
        <button type="button" class="btn btn-lg btn-danger" data-toggle="popover"
        title="Popover title" data-content="This project was developed by Bibi Ruiz"
        @click="onOpen">
        You discovered the Easter Egg!</button>
    </div>
</template>
<script>
// import { EventBus } from '@/utils/eventBus';

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
    onOpen() {
      alert('Hola');
    },
  },
//   data() {
//     return {
//       showMessage: false,
//     };
//   },
//   created() {
//     EventBus.$on('check-counter', console.log('chequeando el counter'));
//   },
//   beforeDestroy() {
//     EventBus.$off('check-counter');
//   },
//   showMessage(counter) {
//     console.log('chequeando el counter', counter);
//     this.showMessage = (counter > 2);
//   },
};
</script>
