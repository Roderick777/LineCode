<template>
<section id="header">
    <header>
        <h1>{{ titulo }}</h1>
        <p>{{ subTitulo }}</p>
    </header>
    <footer>
        <a href="#banner" class="button style2 scrolly-middle">{{ enlace }}</a>
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
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
