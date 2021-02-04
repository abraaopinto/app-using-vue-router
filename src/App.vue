<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/onepage">One Page</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style>
body {
    display: block;
    margin: 0px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: GhostWhite;
  margin: 0px 0px;
}

#nav {
  padding: 30px;
  background: DarkSeaGreen;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: ForestGreen;
}
</style>
