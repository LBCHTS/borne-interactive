<template>
  <el-row :type="flex" :justify="space - between" :align="middle">
    <el-col :span="8">
      <h1 class="titre-principal">Bienvenue chez {{ entreprise }}</h1>
      <router-link  to="/enregistrement">
        <el-button type="primary">S'enregistrer</el-button>
      </router-link>
      <el-link type="primary" icon="el-icon-location">livraison</el-link>
    </el-col>
    <el-col :span="16">
      <el-image :src="image_background" :fit="fill">
        <template #error>
          <div class="image-slot">
            <i class="el-icon-picture-outline"></i>
          </div>
        </template>
      </el-image>
    </el-col>
  </el-row>
</template>

<script>
export default {
  name: "Accueil",
  props: {
    image_background: String,
    entreprise: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.titre-principal {
  font-size: 40px;
}
</style>
