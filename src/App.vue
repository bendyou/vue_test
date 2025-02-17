<template>
  <p :class="{ valid: isValid, disabled: isDisabled }">text</p>
</template>

<script>
export default {
  data() {
    return {
      isValid: true,
      isDisabled: true
    };
  }
}
</script>

<style scoped>
.valid {
  color: green;
}
.disabled {
  color: gray;
}
</style>
