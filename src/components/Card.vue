<template>
<div class="card-custom">
  <div class="card-image is-flex is-horizontal-center">
    <figure class="image">
      <img :src="require(`@/assets/img/${imageTitle}`)" alt="Placeholder image">
    </figure>
  </div>
  <div class="card-content">
    <div class="content">
     {{ text }}
    </div>
  </div>
  <div class="is-flex is-horizontal-center">
       <Button style="width: 60%" buttonText="Learn More"></Button>
  </div>

</div>
</template>

<script>
import Button from './Button.vue'
export default {
  name: 'Card',
  components: {
    Button
  },
    props: [
    'imageTitle',
    'text',
    'buttonText'
    ]
}
</script>
<style>
.card-custom{
    background-color: #fff;
    border-radius: 20px;
    height: 50vh !important;
    min-height: 430px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: top;
}
.is-horizontal-center {
  justify-content: center;
}

.card-content{
    text-align: center;
    font-family: Heebo;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 130%;
}
</style>