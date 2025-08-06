<script>
export default {
  data() {
    return {
      name: 'Hemmie',
      isLoggedIn: false
    };
  },
  methods:
  {
    toggleLogin(){
      this.isLoggedIn = !this.isLoggedIn;
    },
    chnageName(){
      this.name = 'Hemant Dubey';
    }
  }
  
};
</script>

<template>
  <div>
    <h1>Hello, {{ name }}!</h1>
    <input v-model="name" placeholder="Type your name" />

    <p v-if="isLoggedIn">{{name}}, You are logged in</p>
    <p v-else>{{name}}, You are logged out!</p>

    <button @click="toggleLogin">Toggle Login</button>
    <button @click="chnageName">Set name to 'Hemant Dubey'</button>
  </div>
</template>

<style scoped>
input {
  padding: 8px;
  font-size: 16px;
  margin-top: 10px;}
</style>
