<template>
  <p :class="obj">text</p>
</template>

<script>
export default {
  data() {
    return {
      obj: {
        done: true,
        selected: false
      }
    };
  }
}
</script>

<style scoped>
.done {
  color: green;
}
.selected {
  background-color: yellow;
}
</style>
