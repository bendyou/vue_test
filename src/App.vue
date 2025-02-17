<template>
  <div>
    <h1>Task 1</h1>
    <div v-for="elem in items" :key="elem">
      <p>{{ elem }}</p>
      <p class="divider"></p>
    </div>

    <h1>Task 2</h1>
    <ul>
      <li v-for="(elem, index) in items" :key="elem">
        {{ elem }}
      </li>
      <li v-for="(elem, index) in items" :key="'divider' + index" class="divider"></li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [1, 2, 3]
    };
  }
};
</script>
