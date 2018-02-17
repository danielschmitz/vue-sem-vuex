<template>
  <div id="app">
    <button @click="setFakeLogin()">Fake Login</button>
    <button @click="setFakeLogout()">Fake Logout</button>
    <router-view/>
  </div>
</template>

<script>
import store from './store'
export default {
  name: 'App',
  data () {
    return {
      store
    }
  },
  methods: {
    setFakeLogin: function () {
      this.store.username = 'daniel'
      this.store.email = 'daniel@gmail.com'
      this.store.token = 'hdudvo2837hfo2o38f93nknweoi209'
    },
    setFakeLogout: function () {
      this.store.username = ''
      this.store.email = ''
      this.store.token = ''
    }
  }
}
</script>
