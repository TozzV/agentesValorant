<template>
  <div id="app">
    <img v-bind:src="header.url" :alt="header.alt" class="logo">
    <h1 class="header-title">{{ header.titulo }}</h1>


    <navbar>
      <ul></ul>
    </navbar>

    <meu-painel :titulo="foto.titulo">
            <img class="imagem-responsiva" :src="foto.url" :alt="foto.titulo">
    </meu-painel>

    
  </div>
    
</template>

<script>

import Navbar from './components/Navbar.vue';
import agentes from './components/Agentes.vue';

export default {

  components: {
    'navbar' : Navbar,
    
  },
  
  data () {

    return {

      
      header: {   
        titulo: "ESCOLHA O SEU AGENTE",
        url: 'https://www.nse.gg/media/10150/image-4.png?anchor=center&mode=crop&width=300&height=300',
        alt: 'Logo'
      },

      
      }
    }
  }

</script>

<style>

html {
  background-color: #212529;
  font-family: 'Rubik', sans-serif;
}

#app {
  display: flex;
  flex-direction: column;

  color: white;
}

.logo {
  width: 10%;
  margin-top: 2%;
  margin-left: auto;
  margin-right: auto;
}

.header-title {
  text-align: center;
}
</style>
