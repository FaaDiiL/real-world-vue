<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div id="layout">
    <header>
      <div class="wrapper">
        <nav>
          <RouterLink to="/">Events</RouterLink> |
          <RouterLink to="/about">About</RouterLink>
        </nav>
      </div>
    </header>

    <RouterView />
  </div>
</template>

<style lang="scss">
$color_1: #2c3e50;
$color_2: #42b983;
$font-family_1: Avenir, Helvetica, Arial, sans-serif;

#layout {
  font-family: $font-family_1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $color_1;
}
nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: $color_1;
  }
  a.router-link-exact-active {
    color: $color_2;
  }
}
h2 {
  font-size: 20px;
}
</style>
