<template>
  <section>
    <h1 class="titulo">Portfolio</h1>
    <div v-for="(projeto, index) in listaProjetos" :key="index">
      <h2>{{ projeto.nome }}</h2>
      <h3>{{ projeto.titulo }}</h3>
      <img :src="projeto.url_image" alt="imagem" class="imagem">
    </div>
  </section>
</template>

<script>

export default {
  name: 'ProjetoPagina',
  data() {
    return {
      listaProjetos: null
    }
  },
  created() {
  fetch("https://raw.githubusercontent.com/LucasACout/Projetos/main/projetos.json")
    .then(response => response.json())
    .then(data => this.listaProjetos = data);
  }
}

</script>

<style scoped>

.titulo, h2, h3 {
  color: #fff;
}

.titulo {
  text-align: center;
  font-size: 5vw;
  margin-top: 0.5em;
}

h2 {
  font-size: 3vw;
}

h3 {
  font-size: 2vw;
  text-decoration: overline;
}

.imagem {
  width: 100%;
  box-sizing: content-box;
  border-radius: 10px;
}

div {
  margin: 5% 0;
}

</style>