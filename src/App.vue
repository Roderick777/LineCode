<template>
  <div id="app">

    <Cabecera titulo="LineCodify" subTitulo="Te da la Bienvenida" enlace="Hecha un vistazo"/>
    
    <Banner titulo="Soluciones Informáticas" 
    subTitulo="LineCodify te ofrece la posibilidad de llevar tus proyectos a la realidad a través del desarrollo de software con estadares de última técnología" 
    enlace="Mira nuestro Portafolio" />

    <caracteristica titulo="Desarrollo Web" 
    subTitulo="Desarrollo WEB en multiples framework front.end y back-end"
    imagen="./images/pic01.jpg"
    enlace="Mira nuestro Portafolio" />

    <caracteristica titulo="Desarrollo Móvil" 
    subTitulo="Desarrollo de aplicaciones móvil nativas e híbridas"
    imagen="./images/pic02.jpg"
    enlace="Mira nuestro Portafolio" />

    <caracteristica titulo="Desarrollo escritorio"
    subTitulo="Desarrollo de aplicaciones de escritorio multiplataforma"
    imagen="./images/pic02.jpg"
    enlace="Mira nuestro Portafolio" />

    <Portafolio
    titulo="Portafolio" 
    subTitulo="Aquí te damos una pequeña muestra de los ultimos proyectos y trabajos realizados"
    />

    <Contacto
    titulo="Contactanos" 
    subTitulo="¿Deseas realizar una cotización?... ¿Tienes dudas o sugerencias? ... Entonces contactanos para brindarte la mejor guía posible"
    accionForm="#"
    />

    <Pie subTitulo="Linecodify" />

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Cabecera from './components/Cabecera.vue'
import Banner from './components/Banner.vue'
import Caracteristica from './components/Caracteristica.vue'
import Portafolio from './components/Portafolio.vue'
import Contacto from './components/Contacto.vue'
import Pie from './components/Pie.vue'



export default {
  name: 'app',
  components: {
    HelloWorld,
    Cabecera,
    Banner,
    Caracteristica, 
    Portafolio,
    Contacto, 
    Pie
  },
  data(){
    return{
      imagen:{
        caracteristica: ''
      }
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-size: 17px;

  /*margin-top: 60px;*/
}
</style>
