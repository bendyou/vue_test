<template>
  <p :class="cssClasses">text</p>
</template>

<script>
export default {
  data() {
    return {
      cssClasses: 'active valid'
    };
  }
}
</script>

<style scoped>
.active {
  color: red;
}
.valid {
  font-weight: bold;
}
</style>
