<template>
  <div>
    <h1>Task 1</h1>
    <p v-if="!hidden">text</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hidden: true,
    };
  },
};
</script>

<style scoped>
h1 {
  font-size: 24px;
  margin-bottom: 10px;
}
p {
  font-size: 18px;
  margin-top: 10px;
}
</style>
