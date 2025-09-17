<template>

  <Menu></Menu> 
  <Formulario></Formulario>
  <Footer></Footer> 
  <!--<Ejemplo></Ejemplo>-->
  
</template>

<script>
import Menu from './components/menu.vue';
import Formulario from './components/formulario.vue';
import Footer from './components/footer.vue';
//import Ejemplo from './components/ejemplo.vue';


export default {
  name: 'App',
  components: {
    Menu,
    Formulario,
    Footer
    //Ejemplo
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 5px;
}
</style>
