<template>
  <div id="app">
    <Header/>
    <Hero/>
    <div class="p-6 container">
  <div class="columns">
    <div class="column">
      <Card image-title="ic_meditation.svg" text="There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form."/>
    </div>
    <div class="column">
      <Card image-title="ic_yoga.svg" text="It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged."/>
    </div>
    <div class="column">
      <Card image-title="ic_sound.svg" text="It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing."/>
    </div>
  </div>
  </div>
    <Info/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Card from './components/Card.vue'
import Info from './components/Info.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Card,
    Info,
    Footer
  },
    props: [
    'imageTitle',
    'text'
    ]
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html{
  background-color: rgba(230, 248, 245, 1) !important;
  scroll-behavior: smooth;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
