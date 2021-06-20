<template>
  <div id="app">
    <h1 class="text-center" >Habilidades Tecnicas</h1>
    <div class="d-flex justify-content-center">
      <div class="col-2 ">
        <div class="skill">
          <h3 class="text-center fs-4 mb-4 titulos titulo_principal">Sistemas Operativos</h3>
          <div class="container-fluid">
            <p class="titulos text-center text-center">Nodejs + Express.js</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
          <div class="container-fluid">
            <p class="titulos text-center">Angular</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
        </div>
        <div class="skill">
          <h3 class="text-center fs-4 mb-4 titulos titulo_principal">Google Cloud</h3>
          <div class="container-fluid">
            <p class="titulos text-center text-center">Nodejs + Express.js</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
          <div class="container-fluid">
            <p class="titulos text-center">Angular</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-3 skill">
        <h3 class="text-center fs-4 mb-4 titulos titulo_principal">Lenguajes de programación</h3>
        <div class="container-fluid">
          <p class="titulos text-center text-center">Nodejs + Express.js</p>
          <ul class="list-unstyled multi-steps">
            <li></li>
            <li></li>
            <li class="is-active"></li>
            <li></li>
            <li></li>
          </ul>
        </div>
        <div class="container-fluid">
          <p class="titulos text-center">Angular</p>
          <ul class="list-unstyled multi-steps">
            <li></li>
            <li></li>
            <li class="is-active"></li>
            <li></li>
            <li></li>
          </ul>
        </div>
        <div class="container-fluid">
          <p class="titulos text-center">PHP</p>
          <ul class="list-unstyled multi-steps">
            <li></li>
            <li></li>
            <li class="is-active"></li>
            <li></li>
            <li></li>
          </ul>
        </div>
        <div class="container-fluid">
          <p class="titulos text-center">Python</p>
          <ul class="list-unstyled multi-steps">
            <li></li>
            <li></li>
            <li class="is-active"></li>
            <li></li>
            <li></li>
          </ul>
        </div>
      </div>
      <div class="col-2">
        <div class="skill">
          <h3 class="text-center fs-4 mb-4 titulos titulo_principal">Bses de Datos</h3>
          <div class="container-fluid">
            <p class="titulos text-center text-center">Nodejs + Express.js</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
          <div class="container-fluid">
            <p class="titulos text-center">Angular</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
        </div>
        <div class="skill">
          <h3 class="text-center fs-4 mb-4 titulos titulo_principal">Control de Versione Git</h3>
          <div class="container-fluid">
            <p class="titulos text-center text-center">Nodejs + Express.js</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
          <div class="container-fluid">
            <p class="titulos text-center">Angular</p>
            <ul class="list-unstyled multi-steps">
              <li></li>
              <li></li>
              <li class="is-active"></li>
              <li></li>
              <li></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Skills",
  components: {},
};
</script>

<style lang="scss">
$brand-primary: rgb(177, 177, 177);
$white: #fff;
$grey-light: #ededed;
%remain-steps {
  &:before {
    content: counter(stepNum);
    font-family: inherit;
    font-weight: 700;
  }
  &:after {
    background-color: $grey-light;
  }
}
.multi-steps {
  display: table;
  table-layout: fixed;
  width: 100%;
  > li {
    counter-increment: stepNum;
    text-align: center;
    display: table-cell;
    position: relative;
    color: $brand-primary;

    &:before {
      content: "\f00c";
      content: "\2713;";
      content: "\10003";
      content: "\10004";
      content: "\2713";
      display: block;
      margin: 0 auto 4px;
      background-color: $white;
      width: 36px;
      height: 36px;
      line-height: 32px;
      text-align: center;
      font-weight: bold;
      border: {
        width: 2px;
        style: solid;
        color: $brand-primary;
        radius: 50%;
      }
    }
    &:after {
      content: "";
      height: 2px;
      width: 100%;
      background-color: $brand-primary;
      position: absolute;
      top: 16px;
      left: 50%;
      z-index: -1;
    }
    &:last-child {
      &:after {
        display: none;
      }
    }

    &.is-active {
      @extend %remain-steps;
      &:before {
        background-color: $white;
        border-color: $brand-primary;
      }

      ~ li {
        color: #808080;
        @extend %remain-steps;
        &:before {
          background-color: $grey-light;
          border-color: $grey-light;
        }
      }
    }
  }
}

.skill {
  border: 1px solid rgb(37, 8, 8);
  margin: 20px;
  background-color: #424242d0;
  -webkit-box-shadow: 0px 0px 9px 1px rgba(0,0,0,0.56); 
box-shadow: 0px 0px 9px 1px rgba(0,0,0,0.56);
}

.titulos {
  color: white;
}

.titulo_principal{
  padding-top: 50px;
}
</style>