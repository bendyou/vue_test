<template>
  <div>
    <h1>Task 1</h1>
    <ul>
      <template v-for="elem in items" :key="elem">
        <li v-if="elem > 0">{{ elem }}</li>
      </template>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [1, -2, 3, -4, 5]
    };
  }
};
</script>
