<template>
  <div>
    <h1>Task 1</h1>
    <p v-for="num in 30" :key="num">{{ num }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>
