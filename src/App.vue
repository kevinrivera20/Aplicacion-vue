<template>
  <div id="app">
    <div class="navbar-container">
      <div class="navbar-content">
        <div class="icons">
          <router-link active to="/">
            <i class="bx bx-home-alt bx-sm"></i>
          </router-link>
          <router-link active to="/cesta">
            <i class="bx bx-trash bx-sm"></i>
          </router-link>
          <router-link active  to="/favoritos">
            <i class="bx bx-heart bx-sm"></i>
          </router-link>
          <router-link active to="/historial">
            <i class='bx bx-sync bx-sm'></i>
          </router-link>
        </div>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style>

.navbar-container {
  width: 100%;
  position: fixed;
  bottom: 0;
}
.navbar-content {
  padding: 20px;
  display: flex;
  justify-content: space-between;
}

a {
  padding: 27px;
  color: rgba(163, 163, 163);
}

a:hover {
  color: #845EC2;
}


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

* {
    font-family: 'Josefin Sans', sans-serif;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

nav a.router-link-exact-active {
  color: #845EC2;
}
</style>
