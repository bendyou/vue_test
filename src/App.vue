<template>
    <div>
      <h1>Task 1</h1>
      <div>
        <input name="language" type="radio" v-model="choice" value="English"> English
        <input name="language" type="radio" v-model="choice" value="Spanish"> Spanish
        <input name="language" type="radio" v-model="choice" value="French"> French
      </div>
      <p>You choosed: {{ choice }}</p>
  
      <h1>Task 2</h1>
      <div>
        <input name="language" type="radio" v-model="choice" value="English"> English
        <input name="language" type="radio" v-model="choice" value="Spanish"> Spanish
        <input name="language" type="radio" v-model="choice" value="French"> French
      </div>
      <p v-if="choice === 'English'">Hello!</p>
      <p v-if="choice === 'Spanish'">¡Hola!</p>
      <p v-if="choice === 'French'">Bonjour!</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        choice: ''
      };
    }
  };
  </script>
  