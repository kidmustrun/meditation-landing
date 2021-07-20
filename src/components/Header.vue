<template>
  <header>
<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href="#">
      <img src="../assets/img/logo.svg" alt="logo">
    </a>

    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-end">
      <a class="navbar-item">
        Home
      </a>

      <a class="navbar-item">
        Explore
      </a>
      <a class="navbar-item">
        Classes
      </a>
       <a class="navbar-item">
        About Us
      </a>
       <a class="navbar-item">
        Privacy
      </a>
       <a class="navbar-item">
        Services
      </a>
    </div>
  </div>
</nav>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>
<style>
header{
  min-height: 3.25rem;
  background-color: #fff;
  font-family: 'Heebo', sans-serif !important;
}
@media screen and (min-width: 1024px) {
  .navbar{
  padding: 0 3.25rem 0 3.25rem !important
}
}

.navbar-item img {
  height: 3.25rem !important;

}
.navbar-item{
  position: relative;
}
.navbar-item:hover{
  background-color: transparent !important;
  color: #1A7F72 !important;
}
.navbar-item:hover::before {
  position: absolute;
  content: "";
  width: 100%;
  border-bottom: 5px solid #1A7F72;
  bottom: 0;
  left:0;
  border-radius: 10px 10px 0 0;
}
</style>