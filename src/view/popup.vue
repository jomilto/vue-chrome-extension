<template>
  <div class="main_app">
    <h1>Hello {{msg}}</h1>
    <button type="button" @click="show = !show">Mostrar/Ocultar</button>
    <div v-show="show">
      <p>Hola mundo</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'popup',
  data () {
    return {
      msg: 'popup',
      show: true
    }
  }
}

</script>

<style lang="scss" scoped>
@import '~bulma';
.main_app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
