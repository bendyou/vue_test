<template>
  <div>
    <h1>Task 1</h1>
    <p>{{ sqrtResult }}</p>
    <input v-model.number="num" type="number">
    <button v-on:click="calcSqrt">Calculate Square Root</button>

    <h1>Task 2</h1>
    <p>{{ sumResult }}</p>
    <input v-model.number="num1" type="number">
    <input v-model.number="num2" type="number">
    <button v-on:click="calcSum">Calculate Sum</button>

    <h1>Task 3</h1>
    <p>{{ inputText1 }}</p>
    <p>{{ inputText2 }}</p>
    <input v-model="input1">
    <input v-model="input2">
    <button v-on:click="swapText">Swap Text</button>

    <h1>Task 4</h1>
    <p>{{ surname }}</p>
    <p>{{ name }}</p>
    <p>{{ patronymic }}</p>
    <input v-model="fullName">
    <button v-on:click="splitName">Split Name</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      num: 0,
      sqrtResult: 0,
      num1: 0,
      num2: 0,
      sumResult: 0,
      input1: '',
      input2: '',
      inputText1: '',
      inputText2: '',
      fullName: '',
      surname: '',
      name: '',
      patronymic: ''
    };
  },
  methods: {
    calcSqrt() {
      this.sqrtResult = Math.sqrt(this.num);
    },
    calcSum() {
      this.sumResult = this.num1 + this.num2;
    },
    swapText() {
      const temp = this.input1;
      this.input1 = this.input2;
      this.input2 = temp;
    },
    splitName() {
      const nameParts = this.fullName.split(' ');
      this.surname = nameParts[0] || '';
      this.name = nameParts[1] || '';
      this.patronymic = nameParts[2] || '';
    }
  }
};
</script>
