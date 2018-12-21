

<template>
    <article class="container box style3">
        <header>
            <h2 v-html="titulo"></h2>
            <p v-html="subTitulo"></p>
        </header>
        <form method="post" v-bind:action="accionForm">
            <div class="row gtr-50">
                <div class="col-6 col-12-mobile"><input type="text" class="text" name="name" placeholder="Nombre" /></div>
                <div class="col-6 col-12-mobile"><input type="text" class="text" name="email" placeholder="Correo" /></div>
                <div class="col-12">
                    <textarea name="message" placeholder="Mensaje"></textarea>
                </div>
                <div class="col-12">
                    <ul class="actions">
                        <li><input type="submit" value="Contactar" /></li>
                    </ul>
                </div>
            </div>
        </form>
    </article>
</template>

<script>
import { mapState } from 'vuex';

export default {
  name: 'Contacto',
  props: {
    titulo: String,
    subTitulo: String,
    accionForm: String
  }, 
  computed:{
       ...mapState(['tituloApp'])
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
