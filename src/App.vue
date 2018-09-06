<template>
  <div id="app">
    <RouterNav></RouterNav>
    <img id="logo" alt="Vue logo" src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<style scoped lang="scss">
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
  }
  #logo {
    grid-area: logo;
    max-width: 120px;
  }
</style>

<script>
import RouterNav from '@/components/RouterNav.vue'
export default {
  components: {
    RouterNav
  }
}
</script>
