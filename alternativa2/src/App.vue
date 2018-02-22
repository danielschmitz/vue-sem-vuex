<template>
  <div id="app">
    <button @click="setFakeLogin()">Fake Login</button>
    <button @click="setFakeLogout()">Fake Logout</button>
    <router-view/>
  </div>
</template>
<script>
export default {
  name: 'App',
  store: ['username', 'email', 'token'],
  methods: {
    setFakeLogin: function () {
      this.username = 'daniel'
      this.email = 'daniel@gmail.com'
      this.token = 'hdudvo2837hfo2o38f93nknweoi209'
    },
    setFakeLogout: function () {
      this.username = ''
      this.email = ''
      this.token = ''
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
