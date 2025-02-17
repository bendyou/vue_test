<template>
  <div>
    <h1>Task 1</h1>
    <button @click="toggle1">
      {{ visible1 ? 'Hide 1' : 'Show 1' }}
    </button>
    <p v-if="visible1">Text 1</p>

    <button @click="toggle2">
      {{ visible2 ? 'Hide 2' : 'Show 2' }}
    </button>
    <p v-if="visible2">Text 2</p>

    <button @click="toggle3">
      {{ visible3 ? 'Hide 3' : 'Show 3' }}
    </button>
    <p v-if="visible3">Text 3</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible1: false,
      visible2: false,
      visible3: false,
    };
  },
  methods: {
    toggle1() {
      this.visible1 = !this.visible1;
    },
    toggle2() {
      this.visible2 = !this.visible2;
    },
    toggle3() {
      this.visible3 = !this.visible3;
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
