<template>
   <footer class="p-5">
  <div class="content has-text-centered mt-5 p-5">
      <img src="../assets/img/logo.svg" alt="logo">
      <div class="is-flex footer-items">
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
</footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>
<style>
footer{
    background: url("../assets/img/footer-background.svg") 40% 0%;
    background-size: cover;
}
.footer-items{
    justify-content: center;
}
@media screen and (max-width: 520px) {
    .footer-items{
    flex-direction: column;
}
}
</style>