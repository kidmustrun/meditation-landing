<template>
      <button class="button is-rounded button-custom">{{ buttonText }}</button>
</template>

<script>
export default {
  name: 'Button',
  props: [
    'buttonText'
  ]
}
</script>
<style>
.button-custom {
    background-color: rgba(37, 147, 133, 1) !important;
    border: transparent !important;
    color: #fff !important;
    padding: 0 3rem 0 3rem !important;
}
</style>