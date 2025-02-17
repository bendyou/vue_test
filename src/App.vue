<template>
  <div>
    <h1>Task 1</h1>
    <textarea v-model="text"></textarea>
    <p>{{ text }}</p>

    <h1>Task 2</h1>
    <textarea v-model="textAreaContent"></textarea>
    <button v-on:click="convertToArray">Get Words</button>
    <ul>
      <li v-for="(word, index) in words" :key="index">{{ word }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: '',
      textAreaContent: '',
      words: []
    };
  },
  methods: {
    convertToArray() {
      this.words = this.textAreaContent.split(/\s+/);
    }
  }
};
</script>
