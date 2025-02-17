<template>
  <p v-if="age < 18">teenager</p>
  <p v-else-if="age >= 19 && age <= 25">young man</p>
  <p v-else>man</p>
</template>

<script>
export default {
  data() {
    return {
      age: 25,
    };
  },
};
</script>
