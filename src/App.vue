<template>
  <!-- Task 1 -->
  <div>{{ num * num }}</div>

  <!-- Task 2 -->
  <div>{{ num1 + num2 + num3 }}</div>
</template>

<script>
export default {
  data() {
    return {
      num: 5,
      num1: 1,
      num2: 2,
      num3: 3,
    }
  }
}
</script>
