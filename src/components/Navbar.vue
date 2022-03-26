<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#home"
        ><img class="logo" src="../assets/logo.png" alt=""
      /></a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#home">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#about"
              >About</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#createblog">Create a blog</a>
          </li>

          <li class="nav-item">
            <a class="btn" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<script>
export default {};
</script>

<style scoped>
@media screen and (max-width: 678px) {
  .burger {
    display: block;
  }
}
#app {
  color: grey;
}

.btn {
  box-shadow: 1px 1px 15px grey;
  border-radius: 30px;
  font-family: monospace;
  font-size: 20px;
  color: white;
  background-color: #bb313b;
}
.container-fluid {
  z-index: 1;
  background-color: white;
  font-family: monospace;
  font-size: 20px;
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  padding: 0;
  box-shadow: 5px 5px 15px #0e0d0d, -5px -5px 15px #0e0d0d;
}

.logo {
  height: 100px;
  position: relative;
}

#nav a {
  color: #a6776e;
}

#nav a.router-link-exact-active {
  color: #c3a6a1;
}
</style>
