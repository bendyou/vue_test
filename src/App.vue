<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <button @click="showDay">Show Day from Number</button>

    <!-- Task 2 -->
    <h1>Task 2</h1>
    <button @click="showCurrentDay">Show Current Day</button>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    // ¬спомогательный метод, который возвращает день недели по числу
    getDayFromNumber(number) {
      const days = [
        'Sunday', 'Monday', 'Tuesday', 'Wednesday', 
        'Thursday', 'Friday', 'Saturday'
      ];
      return days[number];
    },

    // Task 1: ћетод, который выводит день недели по числу
    showDay() {
      let dayNumber = 3; // Ќапример, 3 - это среда (Wednesday)
      alert(this.getDayFromNumber(dayNumber));
    },

    // Task 2: ќсновной метод, который выводит текущий день недели
    showCurrentDay() {
      const currentDay = new Date().getDay(); // ѕолучаем число текущего дн€ недели
      alert(this.getDayFromNumber(currentDay)); // ¬ыводим название дн€
    }
  }
};
</script>

<style scoped>
h1 {
  font-size: 24px;
  margin-bottom: 10px;
}
button {
  font-size: 18px;
  padding: 10px;
  margin-top: 10px;
}
</style>
