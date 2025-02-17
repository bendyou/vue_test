<template>
  <div>
    <h1>Task 1</h1>
    <ul>
      <li v-for="(elem, key) in obj" :key="key">{{ elem }}</li>
    </ul>

    <h1>Task 2</h1>
    <ul>
      <li v-for="(elem, key) in obj" :key="key">{{ elem }}</li>
    </ul>

    <h1>Task 3</h1>
    <ul>
      <li v-for="(elem, key) in obj" :key="key">{{ key }} - {{ elem }}</li>
    </ul>

    <h1>Task 4</h1>
    <ul>
      <li v-for="(elem, key, index) in obj" :key="key">{{ key }} - {{ elem }} - {{ index }}</li>
    </ul>

    <h1>Task 5</h1>
    <ul>
      <li v-for="(elem, key, index) in obj" :key="key">{{ key }} - {{ elem }} - {{ index + 1 }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: {
        user1: '100$',
        user2: '200$',
        user3: '300$',
      }
    };
  }
};
</script>
