<template>
  <div>
    <p>{{ count }}</p>
    <button @click="increase()">UP</button>
    <button @click="decrease()">DOWN</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: this.initial
    };
  },
  props: {
    initial: {
      type: Number,
      default: 0
    }
  },
  methods: {
    increase() {
      this.count++;
    },
    decrease() {
      this.count--;
    },
  },
};
</script>

<style>
</style>