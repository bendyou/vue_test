<template>
  <div>
    <h1>Task 1</h1>
    <input v-model="message">
    <p>{{ message }}</p>

    <h1>Task 2</h1>
    <input v-model="message">
    <p>{{ message.toUpperCase() }}</p>

    <h1>Task 3</h1>
    <input v-model.number="number" type="number">
    <p>{{ number * number }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: '',
      number: 0
    };
  }
}
</script>
