<template>
      <section class="hero is-fullheight">
<div class="hero-body">
    <div class="container is-max-desktop ">
      <p class="title has-text-centered">
        Practice Wherever You Want, Whenever You Need
      </p>
      <p class="subtitle has-text-centered">
        “These cases are perfectly simple and easy to distinguish. In a free hour, when our power of choice is untrammelled and when nothing prevents our being able to do what we like best.”
      </p>
      <div class="columns">
      <div class="column">
         <img src="../assets/img/practice.svg" alt="Meditation Girl">
      </div>
      <div class="column">
      <Box box-title="Meditation Wind" box-desc="There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form by injected."></Box>
      <Box box-title="Stress Reduction" box-desc="Not again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally can procure him some great pleasure."/>
      <Box box-title="Self Compassion" box-desc="It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s."/>
      </div>
      </div>
    </div>
  </div>
  <div class="hero-body">
    <div class="container is-max-desktop ">
      <p class="title has-text-centered">
        Take a Deep Breath
      </p>
      <p class="subtitle has-text-centered">
        “Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore.”
      </p>
      <div class="columns">
        <div class="column">
     <Sound sound-title="Turning off Auto Pilot" sound-desc="Intriduction, Stress Assesment" sound-src="sound_1.mp3"/>
     <Sound sound-title="Crazy Wind Sound" sound-desc="Relax Mind" sound-src="sound_2.mp3"/>
     <Sound sound-title="Mental Wellness" sound-desc="Stress Relief" sound-src="sound_3.mp3"/>
      </div>
      <div class="column">
         <img src="../assets/img/sound.svg" alt="Meditation Girls">
      </div>
      
      </div>
    </div>
  </div>
</section>
</template>

<script>
import Box from './Box.vue'
import Sound from './Sound.vue'
export default {
  name: 'Info',
  components: {
    Box,
    Sound
  },
  props: [
    'boxTitle',
    'boxDesc',
    'soundTitle',
    'soundDesc',
    'soundSrc'
  ]
}
</script>
<style>

</style>