<template>
  <nav id="router-nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </nav>
</template>

<style scoped lang="scss">
  @import '../scss/_variables';
  $nav-col: #ddd;
  $border-col: darken($nav-col, 7%);
  $btn-height: 4rem;
  #router-nav {
    grid-area: navbar;
    display: grid;
    grid-auto-rows: $btn-height;
    background: $nav-col;
    a {
      padding: 0 1rem;
      line-height: $btn-height;
      font-weight: bold;
      color: #2c3e50;
      border-bottom: 1px solid $border-col;
      background: $nav-col;
      &:hover {
        color: darken($font-col, 10%);
        border-bottom: 0.1em solid darken($border-col, 5%);
        background: darken($nav-col, 5%);}
      // &:focus {
      //   color: darken($font-col, 15%);
      //   border-bottom: 0.1em solid darken($border-col, 15%);}
      &.router-link-exact-active {
        color: $theme-col;
      }
    }
  }
</style>
