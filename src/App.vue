<template>
  <div>
    <h1>Task 1</h1>
    <p>Price: {{ price }}</p>

    <h1>Task 2</h1>
    <button @click="changeCost">Change Cost</button>
    <p>Updated Price: {{ price }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cost: 10,
      amount: 5,
    };
  },
  computed: {
    price() {
      return this.cost * this.amount;
    },
  },
  methods: {
    changeCost() {
      this.cost = 20;
    },
  },
};
</script>

<style scoped>
h1 {
  font-size: 24px;
  margin-bottom: 10px;
}
button {
  font-size: 18px;
  padding: 10px;
  margin-top: 10px;
}
</style>
