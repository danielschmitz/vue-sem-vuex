<template>
  <div class="hello">

    <div v-if="isLogged()">
      Usuário Logado: {{username}}
    </div>
    <div v-else>
      Ninguém logado
    </div>

  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  store: ['username', 'isLogged', 'token']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div{
  padding:30px;
  margin: 10px;
  background: #def;
}
</style>
