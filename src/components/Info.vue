<template>
<div>
      <section class="hero">
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
      </section>
<section class="hero">
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
<section class="hero">
  <div class="hero-body background-waves" style="padding-top: 5rem; padding-bottom: 5rem">
    <div class="container is-max-desktop ">
      <p class="title has-text-centered">
        The Best Of Meditation
      </p>
      <p class="subtitle has-text-centered">
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.”
      </p>
      <div class="columns">
        <div class="column has-text-right">
     <Box box-title="The Peace" box-desc="which of us ever undertakes laborious physical exercise, except to obtain some advantage from it."></Box>
      <Box box-title="Strength Building" box-desc="Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore."/>
      <Box box-title="Quick Relextion" box-desc="It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout."/>
      </div>
      <div class="column has-text-centered image-desktop">
         <img src="../assets/img/best_of_meditation.svg" alt="Meditation Girl" style="height: inherit">
      </div>
      <div class="column has-text-left">
     <Box box-title="Relex & Refresh" box-desc="The generated Lorem Ipsum is therefore always free from repetition, injected humour."></Box>
      <Box box-title="Beauty Of Body" box-desc="Various versions have evolved over the years  sometimes by accident sometimes on purpose injected humour and the like."/>
      <Box box-title="Stress Relief" box-desc="Neque porro quisquam est qui dolorem ipsum quia dolor sit amet consectetur adipisci velit."/>
      </div>
      </div>
    </div>
  </div>
</section>
<section class="hero">
  <div class="hero-body">
    <div class="container is-max-desktop ">
      <p class="title has-text-centered">
       Transform Your Body, Mind and Life Today
      </p>
      <p class="subtitle has-text-centered">
        "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos  sint occaecati cupiditate non provident.”
      </p>
      <div class="columns heebo">
        <div class="column m-5">
     <img src="../assets/img/twisted.svg" alt="Meditation Girl" class="mb-5">
     <p class="is-size-3">
        Backyark Band Meditation
      </p>
      <p class="body-text">
        To take a trivial example, which of us ever undertakes laborious physical exercise except to obtain some advantage from it...<br>
        The generated Lorem Ipsum is therefore always free from repetition, injected humour, or non-characteristic words etc.
      </p>
      <Button button-text="Learn More"/>
      </div>
      <div class="column m-5">
        <p class="is-size-3">
       Antistress Meditation
      </p>
      <p class="body-text">
        There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form by injected.<br>
        These cases are perfectly simple and easy to distinguish. In a free hour when our power of choice is untrammelled.
      </p>
      <Button button-text="Learn More"/>
          <img src="../assets/img/fitness.svg" alt="Meditation Girl" class="mt-5">
      </div>
      
      </div>
    </div>
  </div>
</section>
</div>
</template>

<script>
import Box from './Box.vue'
import Sound from './Sound.vue'
import Button from './Button.vue'
export default {
  name: 'Info',
  components: {
    Box,
    Sound,
    Button
  },
  props: [
    'boxTitle',
    'boxDesc',
    'soundTitle',
    'soundDesc',
    'soundSrc',
    'buttonText'
  ]
}
</script>
<style>
.image-desktop{
    height: 85vh;
  }
@media screen and (max-width: 768px) {
  .image-desktop{
    height: 70vh;
  }
  .column{
    text-align: left !important;
  }
}
.background-waves{
  background: url("../assets/img/background-waves.svg") 0% 0% no-repeat;
  background-size: 100vw 100%;
}
@media screen and (max-width: 1092px) {
  .background-waves{
    background-size: cover;
  }
}
.heebo{
  font-family: Heebo;
}
.body-text{
 color: rgba(0, 0, 0, 0.5);
}
</style>