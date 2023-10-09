<template>
  <div id="container">
    <InfoPagina />
    <ProjetoPagina />
  </div>
</template>

<script>
import InfoPagina from './components/InfoPagina.vue';
import ProjetoPagina from './components/ProjetoPagina.vue';

export default {
  name: 'App',
  components: {
   InfoPagina,
   ProjetoPagina
  }
}
</script>

<style>

@font-face {
  font-family: fonteNova;
  src: url('assets/font/Rajdhani.ttf');
}

* {
  margin: 0;
  padding: 0;
  font-family: fonteNova;
}

@keyframes fundo {
  0%   { background-color: #524096; }
  20%  { background-color: #80ea06; }
  40%  { background-color: #292374; }
  60%  { background-color: #55c302; }
  80%  { background-color: #000551; }
  100% { background-color: #524096; }
}

body {
  background-image: url('assets/fundo.png');
  background-size: 250px 250px;
  background-repeat: repeat;
  animation: fundo 25s infinite;
}

#container {
  max-width: 80vw;
  min-height: 300px;
  background: rgba(0, 0, 0, 40%);
  border-radius: 10px 10px 0px 0px;
  margin: 0 auto;
  margin-top: 30px;
  padding: 25px;
}

</style>
