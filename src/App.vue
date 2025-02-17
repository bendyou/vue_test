<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <p>{{ sum }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: {x: 1, y: 2, z: 3},
    };
  },
  computed: {
    sum() {
      return Object.values(this.obj).reduce((acc, curr) => acc + curr, 0);
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
