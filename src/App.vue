<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">About</router-link>
      <router-link to="/artifacts">Artifacts</router-link>
    </div>
    <div id="container">
      <router-view/>
    </div>
  </div>
</template>

<style lang="scss">
body {
  margin: 0;
}
#app {
  font-family: 'M PLUS 1p', 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  position: fixed;
  width: 100%;
  padding: 16px 0;
  z-index: 10000;
  background-color: #3A3A3A;
  font-size: 18px;
  box-shadow: 0 2px 3px #3A3A3A;
  a {
    margin: 0 10px;
    color: #FFFFFF;
    text-decoration: none;
    .router-link-exact-active {
      font-weight: bold;
      color: #42B983;
    }
  }
}

#nav a {
  font-weight: bold;
  color: #FFFFFF;
}

#nav a.router-link-exact-active {
  color: #42B983;
}

#container {
  padding: 64px 0 0 0;
}

h2 {
  color: #EA8A2A;
}
</style>
