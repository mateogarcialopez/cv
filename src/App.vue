<template>
  <div id="app">
    <div>
      <ul id="menu" class="d-flex justify-content-around">
        <li><a href="#">Acerca</a></li>
        <li><a href="#">Experiencia</a></li>
        <li><a href="#">Habilidades</a></li>
        <li><a href="#">Portafolio</a></li>
        <li><a href="#">Educación</a></li>
      </ul>
      <!--fim menu-->
    </div>
      <About style="margin-bottom: 500px;" />
      <Experience />
  </div>
</template>


<script>
import About from './components/About.vue'
import Experience from './components/Experience.vue'
export default {
  name: "App",
  components: {
    About,
    Experience
  },
};
</script>

<style>
  @import 'assets/styles/styles.scss'
</style>
