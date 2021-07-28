<template>
<section class="hero hero-bg is-fullheight-with-navbar">
<div class="hero-body">
    <div class="container is-max-desktop has-text-centered">
      <p class="title title-hero">
        Meditations Helps You Detoxify Your Body
      </p>
      <p class="subtitle">
        “It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout point of using Lorem Ipsum is that it has a more-or-less.”
      </p>
      <Button button-text="Get Start"/>
      <div class="hero-image">
      <img src="../assets/img/hero-image.svg" alt="Meditation Girl">
      </div>
    </div>
  </div>
</section>
</template>

<script>
import Button from './Button.vue'
export default {
  name: 'Hero',
  components: {
    Button
  },
  props: [
    'buttonText'
  ]
}
</script>
<style>
.hero-bg{
    background: url("../assets/img/hero-bg.svg") bottom;
}
.title{
    font-family: 'Merienda One', cursive !important;  
}
.title-hero{
color: #fff !important;
}
.subtitle{
    color: rgba(0, 0, 0, 0.5) !important;
}
.hero-image img{
    height: 50vh;
    padding-top: 1.25rem;
}
</style>