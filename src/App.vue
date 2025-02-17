<template>
  <div>
    <input type="checkbox" v-model="checked">
    <p>{{ checked ? 'yes' : 'no' }}</p>
    <p v-if="checked">This paragraph is visible because the checkbox is checked.</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checked: true
    };
  }
};
</script>
