<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <button @click="showSquare(2)">Show Square of 2</button>
    <button @click="showSquare(3)">Show Square of 3</button>

    <!-- Task 2 -->
    <h1>Task 2</h1>
    <button @click="showSquare(2)">Square of 2</button>
    <button @click="showSquare(3)">Square of 3</button>
  </div>
</template>

<script>
export default {
  methods: {
    // Task 1: Метод, который выводит квадрат числа
    showSquare(number) {
      alert(number * number);
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
