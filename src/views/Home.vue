<template>
  <div class="app">
    <div class="flex home between">
      <div class="flex">
        <img class="logo" alt="Vue logo" src="../assets/logoblanco.png" height="112px" width="112px" />
      </div>
      <div class="flex">
        <HelloWorld msg="Nombre de la empresa" />
      </div>
    </div>
      <!-- component integration in html code-->
    <div>
      <ImgCabecera />
    </div>
    <div class="fondo-alter">
      <Servicios />
    </div>
    <div class="fondo">
      <ServiciosPar />
    </div>
    <div class="fondo-alter">
      <Texto />
    </div>
    <div class="fondo">
      <Slide/>
    </div>
    <div class="fondo-alter">
      <TextoPar />
    </div>
    <div class="fondo">
      <ImagenTexto />
    </div>
    <div class="fondo-alter">
      <TextoTri />
    </div>
    <div class="fondo">
      <ImagenDchaTexto />
    </div>
    <div class="fondo-alter">
      <TextImgAncho/>
    </div>
    <div class="fondo">
      <Pie />
    </div>
  </div>
</template>

<script>
// import components for integration in html
import HelloWorld from "@/components/HelloWorld.vue";
import ImgCabecera from "@/components/ImgCabecera.vue";
import Servicios from "@/components/Servicios.vue";
import Texto from "@/components/Texto.vue";
import TextoPar from "@/components/TextoPar.vue";
import TextoTri from "@/components/TextoTri.vue";
import ImagenTexto from "@/components/ImagenTexto.vue";
import ImagenDchaTexto from "@/components/ImagenDchaTexto.vue";
import ServiciosPar from "@/components/ServiciosPar.vue";
import Pie from "@/components/Pie.vue";
import Slide from '@/components/Slide.vue';
import TextImgAncho from '@/components/TextImgAncho.vue';

export default {
  name: "Home",
  components: {
    HelloWorld,
    ImgCabecera,
    Servicios,
    Texto,
    TextoPar,
    TextoTri,
    ImagenTexto,
    ImagenDchaTexto,
    ServiciosPar,
    Pie,
    Slide,
    TextImgAncho,
  },
};
</script>

<style lang="scss">

$fondo-oscuro: rgb(39, 39, 39);
$fondo-claro: rgb(255, 255, 255);

.app {
  line-height: 1.7;
  font-family: 'Roboto', sans-serif;
}
.home {
  background-color: $fondo-oscuro;
  display: flex;
  align-items: center;
  padding-left: 10vh;
  padding-right: 10vh;
}
h1, h2, h3 {
  color: rgb(175, 175, 175);
}
h1 {
  font-size: 3rem;
}
h2 {
  font-size: 2rem;
}
h3 {
  font-size: 1.5rem;
}
p {
  font-size: 1rem;
}
.fondo {
  background-color: $fondo-oscuro;
}
.fondo-alter {
  background-color: $fondo-claro;
}
.sombra{
    margin: 10px;
    background-color: $fondo-oscuro;
  /* Sombra normal */
    box-shadow: 2px 2px 10px $fondo-oscuro;
    border-radius: 5px;
    /* Sombra superior sin desenfoque */
    //box-shadow: 5px -5px 0 2px #444;
    /* Sombra interior */
    //box-shadow: 5px 5px 25px #222 inset;
    //background-color: rgb(128, 128, 128);
    //filter: drop-shadow(5px 5px 10px rgb(156, 156, 156));
    
}
.border{
  border-radius: 5px;
}
.limit-1200 {
  max-width: 1200px;
  margin: 0 auto;
}
.limit-1600{
  max-width: 1600px;
  margin: 0 auto;
}
.limit-height{
  width: 100%;
  max-height: 100vh;
}
.flex {
  display: flex;
}
.flex-v {
  flex-direction: row;
}
.flex-h {
  flex-direction: column;
}
.flex .relative {
  position: relative;
}
.flex .absolute {
  position: absolute;
  padding: 10px 10px;
  margin-top: 10vh;
  margin-left: 10vh;
}
.center {
  justify-content: center;
  align-items: center;
}
.center-text {
  align-items: center;
  text-align: center;
}
.left-text {
  align-items: flex-start;
}
.width-33 {
  width: calc(100% / 3);
  min-height: 500px;
}
.width-50 {
  width: calc(100% / 2);
  min-height: 500px;
}
.width-65{
  width: 65%;
  min-height: 500px;
}
.width-35{
  width: 35%;
  min-height: 500px;
}
.separation{
  padding: 10px;
  justify-content: center;
}
.padin-tb-20 {
  padding-top: 20px;
  padding-bottom: 20px;
}
.padin-lr-20 {
  padding-left: 20px;
  padding-right: 20px;
}
.padin-textos {
  padding: 10%;
}
.padin-pie {
  padding: 50px;
}
.width-pie {
  width: calc(100% / 2);
  align-items: center;
}
.between {
  justify-content: space-between;
}
.desktop {
  width: 100%;
}
.separator{
  border-bottom: 1px solid #cacaca;
}

@media  (max-width: 768px){
  .logo{
    width: 56px;
    height: 56px;
  }
  .home {
    padding-left: 1vh;
  }
  img {
    width: 100%;
    max-height: 200px;
  }
  #nombre {
    font-size: 1rem;
  }
  h1{
    font-size: 1.2rem;
  }
  h2{
    font-size: 1rem;
  }
  h3{
    font-size: 0.9rem;
  }
  p {
    font-size: 0.8rem;
  }
  .flex-v{
    flex-direction: column;
    justify-content: center;
  }
  .width-33{
    width: 100%;
    min-height: 0px;
  }
  .width-50 {
    width: 100%;
    min-height: 0px;
  }
  .width-65 {
    width: 100%;
    min-height: 0px;
  }
  .width-35 {
    width: 100%;
    min-height: 0px;
  }
  .limit-1200{
    width: 100%;
    margin: 0;
  }
  .limit-height{
    width: 100%;
    max-height: 100vh;
  }
  .padin-tb-20{
    padding: 10px;
  }
  .padin-lr-20{
    padding: 0px;
  }
  .padin-pie{
    padding: 0;
  }
  .separation {
    padding: 0;
  }
}
</style>
