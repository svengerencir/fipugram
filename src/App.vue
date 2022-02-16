<template>
  <div id="app">
    <div id="nav">
      <router-link class="text-naranca" to="/">Home</router-link> &nbsp
      <router-link class="text-plava" to="/login">Login</router-link> &nbsp
      <router-link class="text-zelena" to="/signup">Signup</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  a {
    font-family: Twiddlestix, Helvetica, Arial, sans-serif;
    font-weight: 600;
    font-size: 1.4rem;
    text-decoration: none;
  }
  padding: 30px;
}
h1,
h2,
h3 {
  font-family: Twiddlestix, Helvetica, Arial, sans-serif;
  margin-bottom: 2rem;
}
label {
  padding-top: 0.5rem;
}
</style>
