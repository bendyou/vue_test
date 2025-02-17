<template>
  <div>
    <p :class="obj">This is some text</p>
    <button @click="showElement">Show</button>
    <button @click="hideElement">Hide</button>
    <button @click="toggleElement">Toggle</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: {
        hidden: true
      }
    };
  },
  methods: {
    showElement() {
      this.obj.hidden = false;
    },
    hideElement() {
      this.obj.hidden = true;
    },
    toggleElement() {
      this.obj.hidden = !this.obj.hidden;
    }
  }
}
</script>

<style scoped>
.hidden {
  display: none;
}
</style>
