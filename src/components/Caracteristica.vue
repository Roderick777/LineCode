<template>
    <article id="first" class="container box style1 right">
        <a href="#" class="image fit"><img :src="imagen" alt="" /></a>
        <div class="inner">
            <header>
                <h2 v-html="titulo"></h2>
            </header>
            <p v-html="subTitulo"></p>
        </div>
    </article>
</template>

<script>
import { mapState } from 'vuex';

export default {
  name: 'Caracteristica',
  props: {
    titulo: String,
    subTitulo: String,
    enlace: String,
    imagen: String
  }, 
  computed:{
       ...mapState(['tituloApp'])
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
