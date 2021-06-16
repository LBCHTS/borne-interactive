<template>
  <Accueil :entreprise="nom" :image_background="image" />
</template>

<script>
import Accueil from '@/components/Accueil'

export default {
  name: "Home",
  components: {
      Accueil,
  },
  setup() {
    const nom = "Caplaser";
    const image = require("../assets/fond_accueil.jpg");

    return {
      nom,
      image,
    };
  },
};
</script>

<style></style>
