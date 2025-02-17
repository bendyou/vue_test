<template>
  <div>
    <h1>Task 1</h1>
    <ul>
      <li v-for="(elem, key) in arr" :key="key">{{ key + 1 }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: ['x', 'y', 'z']
    };
  }
};
</script>
