<template>
  <div>
    <h1>Task 1</h1>
    <p>{{ text }}</p>

    <h1>Task 2</h1>
    <button @click="changeText1">Change Text 1</button>

    <h1>Task 3</h1>
    <button @click="changeText1">Change Text 1</button>
    <button @click="changeText2">Change Text 2</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: 'Initial Text',
    };
  },
  methods: {
    changeText1() {
      this.text = 'Text 1';
    },
    changeText2() {
      this.text = 'Text 2';
    },
  },
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
