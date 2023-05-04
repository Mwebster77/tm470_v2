<template>
  <div>
  <h1>
    Blokzero EOW
  </h1>
</div>

<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <div class="navbar-brand" href="#">
      <img src="./assets/logos/blokzeroLogo.png" alt="Blokzero Logo" width="109" height="28">
    </div>
    <!-- activates the burger menu on small screens -->
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
<!--  Note: Inside of a Vue instance, you have access to the router instance as $router. You can therefore call this.$router.push.
      To navigate to a different URL, use router.push. This method pushes a new entry into the history stack, so when the user clicks the browser back button they will be taken to the previous URL.
      This is the method called internally when you click a <router-link>, so clicking <router-link :to="..."> is the equivalent of calling router.push(...). -->    
          <li class="nav-item">
            <button type="button" class="btn btn-outline-light" @click="$router.push('/')">Dashboard</button>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-outline-light" @click="$router.push('/about')">Tills</button>
          </li>
          <li class="nav-item">
            <div class="btn-group dropend">
              <button type="button" class="btn btn-outline-light">
                Labour
              </button>
              <button type="button" class="btn btn-outline-light dropdown-toggle dropdown-toggle-split" data-bs-toggle="dropdown" aria-expanded="false">
                <span class="visually-hidden">Toggle Dropend</span>
              </button>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" @click="$router.push('')">Wages</a></li>
                <li><a class="dropdown-item" @click="$router.push('')">Forecasting</a></li>
                <li><a class="dropdown-item" @click="$router.push('')">Staff Details</a></li>
              </ul>
            </div>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-outline-light" @click="$router.push('')">Stock</button>
          </li>
          <li class="nav-item">
            <div class="btn-group dropend">
              <button type="button" class="btn btn-outline-light">
                Audit
              </button>
              <button type="button" class="btn btn-outline-light dropdown-toggle dropdown-toggle-split" data-bs-toggle="dropdown" aria-expanded="false">
                <span class="visually-hidden">Toggle Dropend</span>
              </button>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" @click="$router.push('')">Safe Check</a></li>
                <li><a class="dropdown-item" @click="$router.push('')">FOH Checks</a></li>
                <li><a class="dropdown-item" @click="$router.push('')">BOH Checks</a></li>
                <li><hr class="dropdown-divider"></li>
                <li><a class="dropdown-item" @click="$router.push('')">New incident</a></li>
                <li><a class="dropdown-item" @click="$router.push('')">View incidents</a></li>
              </ul>
            </div>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-outline-light" @click="$router.push('')">Purchases</button>
          </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
<router-view/>

</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

.navbar-nav > li{
  padding-left: 1.5px;
  padding-right: 1.5px;
}

.navbar{
  background-color: #b0bec5;
}

</style>
