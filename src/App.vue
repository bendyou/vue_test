<template>
  <div>
    <p v-if="day === 'Monday'">Monday</p>
    <p v-if="day === 'Tuesday'">Tuesday</p>
    <p v-if="day === 'Wednesday'">Wednesday</p>
    <p v-if="day === 'Thursday'">Thursday</p>
    <p v-if="day === 'Friday'">Friday</p>
    <p v-if="day === 'Saturday'">Saturday</p>
    <p v-if="day === 'Sunday'">Sunday</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      day: 'Wednesday',
    };
  },
};
</script>

<style scoped>
p {
  font-size: 18px;
  margin-top: 10px;
}
</style>
