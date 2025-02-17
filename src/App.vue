<template>
  <p :class="{ active: true, valid: false }">text</p>
</template>

<script>
export default {
  data() {
    return {};
  }
}
</script>

<style scoped>
.active {
  color: green;
}
.valid {
  font-weight: bold;
}
</style>
