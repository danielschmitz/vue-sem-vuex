<template>
  <div class="hello">

    <div v-if="store.isLogged()">
      Usuário Logado: {{store.username}}
    </div>
    <div v-else>
      Ninguém logado
    </div>

  </div>
</template>

<script>

import store from '../store'

export default {
  name: 'HelloWorld',
  data () {
    return {
      store
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div{
  padding:30px;
  background: #def;
}
</style>
