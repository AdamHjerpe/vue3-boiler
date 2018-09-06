<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>
</template>

<style scoped lang="scss">
  #nav {
    grid-area: nav;
    padding: 3em 0;
    a {
      padding: 0 1em 0 0;
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
</style>
