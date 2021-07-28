<template>
      <div class="box">
          <div class="columns is-mobile">
              <div class="column is-three-quarters">
<strong>{{ soundTitle }}</strong><br>
            <p> {{ soundDesc }} </p>
              </div>
              <div class="column ">
<audio :id="soundSrc" :src="require(`@/assets/audio/${soundSrc}`)"></audio>
<button :id="soundSrc + '_button'" class="sound-button" @click="soundClick()"><i :id="soundSrc + '_i'" class="material-icons">play_arrow</i></button>
              </div>
          </div>
            
            
        </div>
</template>

<script>

export default {
  name: 'Box',
      
  props: [
    'soundTitle',
    'soundDesc',
    'soundSrc'
  ],
  methods: {
soundClick() {
    var audio = document.getElementById(this.soundSrc);
    var button_i = document.getElementById(this.soundSrc + '_i');
    var button = document.getElementById(this.soundSrc + '_button');
    var audios = document.getElementsByTagName('audio');
        if(!audio.paused){
        audio.pause();
        button_i.innerHTML = 'play_arrow'
        button.style.opacity = 0.7; 
    } else {
        audio.play();
        button_i.innerHTML = 'pause'
        button.style.opacity = 1;
    }
    for(var i = 0; i < audios.length; i++) {
        if(audios[i] !=audio){
        audios[i].pause();
        audios[i].currentTime = 0;
        for (let sibling of audios[i].parentNode.children) {
        sibling.style.opacity = 0.7;
        for (let icon of sibling.childNodes)
        icon.innerHTML = 'play_arrow'
            }
} 
  }
},
  }
}
</script>
<style>
.box{
    background: linear-gradient(90deg, #C3E2DE 27.22%, #CFF1ED 48.89%, #EDFBF9 96.77%) !important;
    border-radius: 15px !important;
    box-shadow: none;
}
.sound-button{
    padding: 0 !important; 
    border-radius: 100%; 
    width: 40px; 
    height: 40px;
    opacity: 0.7;
    background: linear-gradient(180deg, #259385 0%, #159685 100%);
    box-shadow: 0px 25px 30px rgba(179, 228, 221, 0.3), 0px 9px 24px rgba(26, 127, 114, 0.23);
    border: none;
    color: #fff;
    transition: all 0.2s ease-in-out;
}
.sound-button:hover{
    opacity: 1;
    transition: all 0.2s ease-in-out;
}
</style>