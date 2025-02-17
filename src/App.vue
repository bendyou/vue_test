<template>
  <div>
    <h1>Task 1</h1>
    <select v-model="selectedCity">
      <option>New York</option>
      <option>Los Angeles</option>
      <option>Chicago</option>
    </select>
    <p>{{ selectedCity }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedCity: 'New York',
    };
  },
};
</script>
