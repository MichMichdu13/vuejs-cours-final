<template>
  <div class="concerts">
    <BannerConcert :bannerData= "texteConcert.bannerData"/>
    <CardStyleMusic :titleCardStyle= "texteConcert.slider.titleSlider.titleCardStyle1" />
    <CardStyleMusic :titleCardStyle= "texteConcert.slider.titleSlider.titleCardStyle2" />
    <CardStyleMusic :titleCardStyle= "texteConcert.slider.titleSlider.titleCardStyle3" />
  </div>
</template>

<script>

import BannerConcert from '../components/concert/bannerConcert.vue';
import CardStyleMusic from '../components/concert/cardStyleMusic.vue';

export default {
  name: 'Concerts',
  components: {
    BannerConcert,
    CardStyleMusic,

  },
  data() {
    return {
      texteConcert: {
        bannerData:{
          mainTitreData:{
            titre1homeData: "Tout les concerts,",
            soustitre1homeData: "en avant-première.",
          },
        },
        slider:{
          titleSlider:{
            titleCardStyle1:"Rap/Rnb",
            titleCardStyle2:"Variété française",
            titleCardStyle3:"Electro",
          }
        }
      }
    }
  }
}

</script>

<style lang="scss">
.concerts {
  color: white;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

}
</style>