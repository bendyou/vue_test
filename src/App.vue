<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <p>{{ arr2[0] }}</p>
    <p>{{ arr2[1] }}</p>
    <p>{{ arr2[2] }}</p>

    <!-- Task 2 -->
    <h1>Task 2</h1>
    <p>{{ sum }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr2: ['x', 'y', 'z'],
      arr: [1, 2, 3]
    };
  },
  computed: {
    sum() {
      return this.arr.reduce((acc, curr) => acc + curr, 0);
    }
  }
};
</script>

<style scoped>
h1 {
  font-size: 24px;
  margin-bottom: 10px;
}
p {
  font-size: 18px;
}
</style>
