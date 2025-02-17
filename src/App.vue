<template>
  <div>
    <h1>Task 1</h1>
    <div v-for="item in items" :key="item">{{ item }}</div>
    
    <h1>Task 2</h1>
    <div v-for="item in items" :key="item">{{ item * item }}</div>

    <h1>Task 3</h1>
    <ul>
      <li v-for="item in items" :key="item">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [1, 2, 3, 4, 5]
    };
  }
};
</script>
