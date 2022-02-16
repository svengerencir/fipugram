<template>
  <div id="app">
    <nav
      id="nav"
      class="navbar navbar-expand-lg navbar-light fixed-top bg-white"
    >
      <router-link class="text-naranca navbar-brand" to="/">
        <img
          src="@/assets/logo.png"
          width="40px"
          height="40px"
          class="d-inline-block align-center"
          alt=""
          loading="lazy"
        />
        fipugram
      </router-link>
      <button
        class="navbar-toggler btn-naranca"
        type="button"
        data-toggle="collapse"
        data-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse float-right" id="navbarNav">
        <ul class="navbar-nav mr-1 ml-auto">
          <li class="nav-item">
            <router-link class="text-naranca" to="/"> home &ensp;</router-link>
          </li>
          <li class="nav-item">
            <router-link class="text-plava" to="/login"
              >Login &ensp;</router-link
            >
          </li>
          <li class="nav-item">
            <router-link class="text-zelena" to="/signup"
              >Signup &ensp;</router-link
            >
          </li>
        </ul>
        <form class="form-inline">
          <input
            class="form-control funfont btn-roza border-roza"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
        </form>
      </div>
    </nav>
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
    font-size: 1.5rem;
    text-decoration: none;
  }
  padding: 30px;
}
.navbar-toggler {
  outline: none !important;
}
.funfont {
  font-family: Twiddlestix, Helvetica, Arial, sans-serif;
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
body {
  padding-top: 96px;
  overflow-x: hidden;
}
html {
  scroll-behavior: smooth;
}
</style>
