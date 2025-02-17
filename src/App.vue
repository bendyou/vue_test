<template>
  <div>
    <input type="checkbox" v-model="languages" value="English"> English
    <input type="checkbox" v-model="languages" value="Spanish"> Spanish
    <input type="checkbox" v-model="languages" value="French"> French
    <input type="checkbox" v-model="languages" value="German"> German
    <ul>
      <li v-for="(language, index) in languages" :key="index">{{ language }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      languages: [],
    };
  },
};
</script>
