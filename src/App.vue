<script>
export default {
  data() {
    return {
      name: 'Hemmie'
    };
  }
};
</script>

<template>
  <div>
    <h1>Hello, {{ name }}!</h1>
    <input v-model="name" placeholder="Type your name" />
  </div>
</template>

<style scoped>
input {
  padding: 8px;
  font-size: 16px;
  margin-top: 10px;}
</style>
