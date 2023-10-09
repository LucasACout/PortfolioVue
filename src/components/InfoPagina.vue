<template>
  <section>
    <h1>Lucas de Andrade</h1>
    <div class="foto">
      <img src="../assets/foto.png" alt="foto">
    </div>
    <div class="info">
      <p><b>Nome: </b>Lucas de Andrade Coutinho Arruda</p>
      <p><b>Data de nascimento: </b>10/11/2000</p>
      <p><b>Nacionalidade: </b>Brasileiro</p>
      <p><b>GitHub: </b><a href="https://github.com/LucasACout">LucasACout</a></p>
      <p><b>LinkedIn: </b><a href="https://www.linkedin.com/in/lucas-andrade-550b61198/">Lucas Andrade</a></p>
    </div>
    <hr>
  </section>
</template>

<script>
  export default {
    name: 'InfoPagina'
  }
</script>

<style scoped>

h1, h2, p {
  color: #fff;
}

h1 {
  font-size: 6vw;
  text-align: center;
}

p {
  font-size: 1.2em;
}

.info {
  margin: 25px 0px;
}

h2 {
  font-size: 4vw;
}

a {
  color: #fff;
  text-decoration: none;
  border-right: 5px solid #fff;
  padding-right: 5px;
}

section {
  position: relative;
}

.foto img {
  display: none;
  border-radius: 100%;
  border: 5px solid #fff;
  width: 17%;
  position: absolute;
  top: 0;
  right: 0;
}

@media screen and (min-width: 800px) {
  .foto img {
    display: block;
  }
}

</style>