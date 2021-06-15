<template>
  <div>
    <div
      class="colormain"
      id="aboutBoxPrimary"
      style="border 1px solid red"
    ></div>
    <div id="about" class="d-flex flex-column align-items-center">
      <div>
        <h3 class="letra">Mateo García López</h3>
      </div>
      <div>
        <h4 class="letra">Desarrollador Web</h4>
      </div>
      <div id="photo" class="d-flex flex-column align-items-center">
        <img src="../assets/img/foto003.jpeg" alt="" />
      </div>
      <div
        class="card d-flex flex-column align-items-center px-5 pb-3"
        id="aboutMe"
      >
        <div id="icons">
          <a
            href="https://www.facebook.com/mateo.garcialopez.1/"
            target="_blank"
            ><i class="bi bi-facebook"></i
          ></a>
          <a
            href="https://www.linkedin.com/in/mateo-garc%C3%ADa-l%C3%B3pez-7358a7139/"
            target="_blank"
            ><i class="bi bi-linkedin"></i
          ></a>
          <a href="https://github.com/mateogarcialopez"
            ><i class="bi bi-github" target="_blank"></i
          ></a>
        </div>
        <div>
          <p class="letra">
            Ingeniero de sistemas y telecomunicaciones, en capacidad de proponer
            soluciones acordes a las necesidades empresariales, sin dejar a un
            lado la responsabilidad ética, conocer y asumir posiciones críticas
            sobre las normas y políticas en el campo de los sistemas, capaz de
            proponer y generar ideas innovadoras que permitan la creación de
            nuevas soluciones tecnológicas, saber adaptar sus conocimientos y
            habilidades a las nuevas tecnologías.
          </p>
        </div>
        <div class="btn">
          <button class="btn btn-success">Descargar CV</button>
          <button class="btn btn-success">Contactame</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  components: {},
};
</script>

<style>
@import "../assets/styles/styles.scss";
#aboutBoxPrimary {
  height: 200px;
  width: 100%;
  -webkit-box-shadow: -1px 3px 11px 1px rgba(0, 0, 0, 0.48);
  box-shadow: -1px 3px 11px 1px rgba(0, 0, 0, 0.48);
}

#icons a {
  margin: 5px;
  font-size: 30px;
  color: rgb(41, 53, 42);
}

#photo img {
  border-radius: 100%;
  border: 3px solid rgb(153, 146, 146);
  width: 195px;
  position: absolute;
  height: 210px;
  top: 19%;
  z-index: 999;
}

#about {
  top: 83px;
  width: 60%;
  position: absolute;
  left: 0;
  right: 0;
  margin-left: auto;
  margin-right: auto;
}

.letra {
  color: rgb(160, 158, 158);
  font-family: "Courier New", Courier, monospace;
  text-align: justify;
}

#aboutMe {
  margin-top: 110px;
  padding-top: 150px;
  -webkit-box-shadow: -1px 3px 11px 1px rgba(0, 0, 0, 0.48);
  box-shadow: -1px 3px 11px 1px rgba(0, 0, 0, 0.48);
}

.btn{
    margin: 3px;
}
</style>