<template>
    <section id="footer">
        <ul class="icons">
            <li><a href="#" class="icon fa-twitter"><span class="label">Twitter</span></a></li>
            <li><a href="#" class="icon fa-facebook"><span class="label">Facebook</span></a></li>
            <li><a href="#" class="icon fa-google-plus"><span class="label">Google+</span></a></li>
            <li><a href="#" class="icon fa-pinterest"><span class="label">Pinterest</span></a></li>
            <li><a href="#" class="icon fa-dribbble"><span class="label">Dribbble</span></a></li>
            <li><a href="#" class="icon fa-linkedin"><span class="label">LinkedIn</span></a></li>
            <font-awesome-icon icon="coffee" />
        </ul>
        <div class="copyright">
            <ul class="menu">
                <li v-html="subTitulo"></li>
            </ul>
        </div>
    </section>
</template>

<script>
import { mapState } from 'vuex';

export default {
  name: 'Pie',
  props: {
    subTitulo: String,
  }, 
  computed:{
       ...mapState(['tituloApp'])
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
