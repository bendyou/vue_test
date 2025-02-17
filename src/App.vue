<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <button @click="showSum">Show Sum</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      num1: 1,
      num2: 2
    };
  },
  methods: {
    showSum() {
      alert(this.num1 + this.num2);
    }
  }
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
