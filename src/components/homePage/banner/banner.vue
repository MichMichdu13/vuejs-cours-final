<template>
  <div class="banner">
      <titleMainHome :title1="bannerData.mainTitreData.titre1homeData" :title2="bannerData.mainTitreData.soustitre1homeData"/>
      <carouselle :topConcerts = "topConcerts"/>
      <title2home :title3="bannerData.titre2homeData"/>
      <bigEtape :bigEtapeData="bannerData.bigEtapeData"/>
  </div>
</template>

<script>
import carouselle from './carouselle.vue'
import titleMainHome from './titleMain.vue'
import title2home from './titre2home.vue'
import bigEtape from './bigEtape.vue'

export default {
  name: 'banner',
  components: {
    titleMainHome,
    carouselle,
    title2home,
    bigEtape,
  },
    props: {
    topConcerts: Array,
    bannerData: Object,

  },
}
</script>
<style lang="scss">
    .banner{
        background: radial-gradient(51.9% 336.54% at 51.9% 50%, #241B4D 0%, #1B1B1B 100%);
        border-radius: 0px 0px 150px 150px;
    }
</style>
