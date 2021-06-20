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
      <Skills/>
  </div>
</template>


<script>
import About from './components/About.vue'
import Experience from './components/Experience.vue'
import Skills from './components/skill.vue'
export default {
  name: "App",
  components: {
    About,
    Experience,
    Skills
  },
};
</script>

<style>
  @import 'assets/styles/styles.scss'
</style>
