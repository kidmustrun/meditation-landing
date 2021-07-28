<template>
      <div class="box">
            <strong>{{ boxTitle }}</strong><br>
            <p> {{ boxDesc }} </p>
        </div>
</template>

<script>
export default {
  name: 'Box',
  props: [
    'boxTitle',
    'boxDesc'
  ]
}
</script>
<style>
.box{
    background-color: rgba(255, 255, 255, 0.5) !important;
    cursor: pointer;
    transition: all 0.2s ease-in-out;
}
.box:hover{
    background-color: white !important;
    transition: all 0.4s ease-in-out;
}
</style>