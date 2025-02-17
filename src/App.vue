<template>
  <div>
    <h1>Task 1</h1>
    <button @click="show">Show</button>
    <p v-if="visible">text</p>

    <h1>Task 2</h1>
    <button @click="show">Show</button>
    <button @click="hide">Hide</button>
    <p v-if="visible">text</p>

    <h1>Task 3</h1>
    <button v-if="!visible" @click="show">Show</button>
    <button v-if="visible" @click="hide">Hide</button>
    <p v-if="visible">text</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: false,
    };
  },
  methods: {
    show() {
      this.visible = true;
    },
    hide() {
      this.visible = false;
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
p {
  font-size: 18px;
  margin-top: 10px;
}
</style>
