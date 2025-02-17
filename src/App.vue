<template>
  <button @click="toggle">Toggle</button>
  <p v-show="isVisible">Text</p>
</template>

<script>
export default {
  data() {
    return {
      isVisible: true,
    };
  },
  methods: {
    toggle() {
      this.isVisible = !this.isVisible;
    },
  },
};
</script>
