<template>
<<<<<<< HEAD
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
=======
  <main class="columns is-gapless is-multiline" :class="{'modo-escuro': modoEscuroAtivo}">
      <div class="column is-one-quarter">
          <BarraLateral @aoTemaAlterado="trocarTema"/>
      </div>
      <div class="column is-three-quarter conteudo">
          <router-view></router-view>
      </div>
  </main>
>>>>>>> dcde9eb (adasdasdsadsada)
</template>

<script lang="ts">
import { defineComponent } from 'vue';
<<<<<<< HEAD
import HelloWorld from './components/HelloWorld.vue';

export default defineComponent({
  name: 'App',
  components: {
    HelloWorld
=======
import BarraLateral from "@/components/BarraLateral.vue";

export default defineComponent({
  name: 'App',
  components: {BarraLateral},
  data(){
    return {
       modoEscuroAtivo: false
    }
  },
  methods:{
    trocarTema(modoEscuroAtivo: boolean){
      this.modoEscuroAtivo = modoEscuroAtivo;
    }
>>>>>>> dcde9eb (adasdasdsadsada)
  }
});
</script>

<<<<<<< HEAD
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
=======
<style scoped>
  main {
    --bg-primario: #FFF;
    --texto-primario: #000;
  }

  main.modo-escuro{
    --bg-primario: #2b1d42;
    --texto-primario: #ddd;
  }

  .conteudo{
    background-color: var(--bg-primario);
  }
>>>>>>> dcde9eb (adasdasdsadsada)
</style>
