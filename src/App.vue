<template>
  <button @click="hide">Hide</button>
  <template v-if="isVisible">
    <p>Text 1</p>
    <p>Text 2</p>
    <p>Text 3</p>
  </template>
</template>

<script>
export default {
  data() {
    return {
      isVisible: true,
    };
  },
  methods: {
    hide() {
      this.isVisible = false;
    },
  },
};
</script>
