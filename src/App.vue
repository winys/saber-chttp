<template>
  <div id="app">
     <link rel="stylesheet" :href="theme_addr">
    <saber_chttp></saber_chttp>
  </div>
</template>

<script>
import saber_chttp from './components/saber_chttp'

export default {
  name: 'app',
  components: {
    saber_chttp
  },
  computed: {
      theme_addr () {return "../../app/static/css/" + Saber.preferences.theme +".css";}
  }
}
</script>

<style>
html,body,#app{
  height: 100%;
  width: 100%;
}
*{
  margin: 0;
  padding: 0;
}
</style>
