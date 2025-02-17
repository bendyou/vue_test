<template>
  <div>
    <h1>Task 1</h1>
    <a href="https://example.com" @click.prevent="handleClick">Click me</a>

    <h1>Task 2</h1>
    <button @click.once="handleClickOnce">Click me once</button>
  </div>
</template>

<script>
export default {
  methods: {
    handleClick() {
      alert('Link clicked!');
    },
    handleClickOnce() {
      alert('Button clicked once!');
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
