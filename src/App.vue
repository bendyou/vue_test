<template>
  <div>
    <h1>Task 1</h1>
    <ul>
      <li v-for="elem in arr" :key="elem">{{ elem }}</li>
    </ul>
    <button @click="addItem">Add Item</button>

    <h1>Task 2</h1>
    <ul>
      <li v-for="elem in arr" :key="elem">{{ elem }}</li>
    </ul>
    <button @click="removeFirst">Remove First</button>

    <h1>Task 3</h1>
    <ul>
      <li v-for="elem in arr" :key="elem">{{ elem }}</li>
    </ul>
    <button @click="removeLast">Remove Last</button>

    <h1>Task 4</h1>
    <ul>
      <li v-for="elem in arr" :key="elem">{{ elem }}</li>
    </ul>
    <button @click="removeSecondLast">Remove Second Last</button>

    <h1>Task 5</h1>
    <ul>
      <li v-for="elem in arr" :key="elem">{{ elem }}</li>
    </ul>
    <button @click="sortList">Sort List</button>

    <h1>Task 6</h1>
    <ul>
      <li v-for="elem in arr" :key="elem">{{ elem }}</li>
    </ul>
    <button @click="reverseList">Reverse List</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: ['a', 'b', 'c'],
    };
  },
  methods: {
    addItem() {
      this.arr.push('new item');
    },
    removeFirst() {
      this.arr.shift();
    },
    removeLast() {
      this.arr.pop();
    },
    removeSecondLast() {
      this.arr.splice(this.arr.length - 2, 1);
    },
    sortList() {
      this.arr.sort();
    },
    reverseList() {
      this.arr.reverse();
    }
  }
}
</script>
