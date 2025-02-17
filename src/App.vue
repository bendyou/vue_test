<template>
  <div>
    <h1>Task 1</h1>
    <p v-if="isAdmin">You have admin privileges</p>
    <p v-else>You do not have admin privileges</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isAdmin: true,
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
