<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <button @click="showDate">Show Date</button>
  </div>
</template>

<script>
export default {
  methods: {
    showDate() {
      alert(new Date());
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
