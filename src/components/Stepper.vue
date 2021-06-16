<template>
  <el-steps :active="0" align-center>
    <el-step title="Présentez-vous">
      <!--<Presentation />-->
      
    </el-step>
    <el-step title="Qui visitez-vous aujourd'hui">
      <!--<RendezVous />-->
    </el-step>
    <el-step title="Récapitulatif">
      <!--<Recapitulatif />-->
    </el-step>
  </el-steps>
</template>

<script>
//import Presentation from "./Presentation.vue";
//import RendezVous from "./RendezVous.vue";
//import Recapitulatif from "./Recapitulatif.vue";

export default {
  name: "Stepper",
  components: {
    //Presentation,
    //RendezVous,
    //Recapitulatif,
  },
};
</script>

<style></style>
