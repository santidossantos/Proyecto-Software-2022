<template>
  <h1 class="title">Estadisticas</h1>
  <div class="est">
    <Estadisticas />
    <EstadisticasGenero />
    <EstadisticasInscripciones />
  </div>
  <hr class="hr" />
</template>

<script>
// @ is an alias to /src
import Estadisticas from "@/components/Estadisticas.vue";
import EstadisticasGenero from "@/components/EstadisticasGenero.vue";
import EstadisticasInscripciones from "@/components/EstadisticasInscripciones.vue";

export default {
  name: "StatisticsView",
  components: {
    Estadisticas,
    EstadisticasGenero,
    EstadisticasInscripciones,
  },
};
</script>

<style>
.est {
  display: flex;
  flex-direction: row;
  gap: 5rem;
  padding: 4rem;
  column-span: none;
}

@media screen and (max-width: 510px) {
  .est {
    display: flex;
    flex-direction: column;
  }
}

.hr {
  width: 70%;
  margin: auto;
  justify-content: center;
}
</style>
