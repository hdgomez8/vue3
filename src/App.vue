<script setup>
import fundamentos from "@/assets/images/fundamentos.png";
import miPrimerProyecto from "@/assets/images/miPrimerProyecto.png";
import sintaxis from "@/assets/images/sintaxis.png";
import interpolacionTexto from "@/assets/images/interpolacionTexto.png";
import enlacesDeAtributos from "@/assets/images/enlacesDeAtributos.png";
import expresionesJS from "@/assets/images/expresionesJS.png";
import directivas from "@/assets/images/directivas.png";
import vIf from "@/assets/images/v-if.png";
import vElse from "@/assets/images/v-else.png";
import vElseIncorrecto from "@/assets/images/v-else-incorrecto.png";

//2-Interpolacion De Texto
const name = "Héctor Gómez";
//3-Enlaces De Atributos
const styleColor = "color:red;";
</script>

<!-- 1-Sintaxis De Plantilla -->
<template>
  <!-- 2-Interpolacion De Texto -->
  <h1>Hola {{ name }}!</h1>

  <!-- 3-Enlaces De Atributos - Sintaxis Normal -->
  <h2 v-bind:style="styleColor">Hola {{ name }}</h2>
  <!-- 3-Enlaces De Atributos - Sintaxis Abreviada -->
  <h2 :style="styleColor">Hola {{ name }}</h2>

  <div>
    <div class="gray-background">
      <h1>Fundamentos</h1>
      <img :src="fundamentos" alt="fundamentos" />
    </div>
    <div class="gray-background2">
      <h1>Mi Primer Proyecto</h1>
      <img :src="miPrimerProyecto" alt="miPrimerProyecto" />
    </div>
    <div class="gray-background">
      <h1>Sintaxis</h1>
      <img :src="sintaxis" alt="sintaxis" />
    </div>
    <div class="gray-background2">
      <h1>Interpolacion De Texto</h1>
      <img :src="interpolacionTexto" alt="interpolacionTexto" />
    </div>
    <div class="gray-background">
      <h1>Enlace De Atributos</h1>
      <img :src="enlacesDeAtributos" alt="enlacesDeAtributos" />
    </div>
    <div class="gray-background2">
      <h1>Expresiones JS</h1>
      <img :src="expresionesJS" alt="expresionesJS" />
    </div>
    <div class="gray-background">
      <h1>Directivas</h1>
      <img :src="directivas" alt="directivas" />
    </div>
    <div class="gray-background2">
      <h1>V-If</h1>
      <img :src="vIf" alt="vIf" />
    </div>
    <div class="gray-background">
      <h1>V-Else</h1>
      <img :src="vElse" alt="vElse" />
      <img :src="vElseIncorrecto" alt="vElseIncorrecto" />
    </div>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}

.gray-background {
  background-color: #f0f0f0; /* Establece el color de fondo en gris */
  padding: 20px; /* Añade un relleno alrededor del contenido del div */
}

.gray-background2 {
  background-color: #b0b0b0; /* Establece el color de fondo en gris */
  padding: 20px; /* Añade un relleno alrededor del contenido del div */
}
</style>
