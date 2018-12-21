<template>
    <section id="banner">
        <header>
            <h2>{{ titulo }}</h2>
        </header>
        <p v-html="subTituloComp"></p>
        <footer>
            <a href="#first" class="button style2 scrolly">{{ enlace }}</a>
        </footer>
    </section>
</template>

<script>
import { mapState } from 'vuex';

export default {
  name: 'Cabecera',
  props: {
    titulo: String,
    subTitulo: String,
    enlace: String
  }, 
  computed:{
       ...mapState(['tituloApp'])
  },
  data(){
      return{
          subTituloComp: this.subTitulo
      } 
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
