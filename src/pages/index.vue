<template>
  <div class="home">
    <banner :topConcerts = "topConcerts" :bannerData= "texteSite.bannerData"/>
    <phone :phoneData="texteSite.phoneData"/>
  </div>
</template>

<script>
import banner from '../components/homePage/banner/banner.vue';
import phone from '../components/homePage/phone.vue';
export default {
  name: 'Home',
  components: {
    banner,
    phone,
  },
data() {
    return {
      texteSite: {
        bannerData:{
          mainTitreData:{
            titre1homeData: "Les meilleurs concerts,",
            soustitre1homeData: "en avant-première.",
          },
          titre2homeData: "buuk, le rêve des fans de concerts.",
          bigEtapeData:{
            etape1Data:{
              number:"1",
              titre:"Choisis ton artiste",
              text:"Nous te proposons régulièrement des concerts en avant-première, choisis le concert de ton artiste préféré parmi ceux proposés"
            },
            etape2Data:{
              number:"2",
              titre:"Réserve ton billet",
              text:"buuk te propose les prix les plus attractifs du marché, plus tu réserve tôt, plus tu auras droit à un prix bas. Alors fonce, ne perds pas de temps !"
            },
            etape3Data:{
              number:"3",
              titre:"Kiffe ton concert",
              text:"Nous te proposons régulièrement des concerts en avant-première, choisis le concert de ton artiste préféré parmi ceux proposés"
            }
          }
        },
        phoneData:{
          phoneTiteData: "buuk, aussi sur ton téléphone !",
          phonetextData: "Télécharge l’application book sur ton smartphone pour pouvoir réserver encore plus facilement et être tenu au courant grâce aux notifications des derniers concerts disponibles sur la plateforme",
        },


      },
      topConcerts: [
        {id: "angele", name: "Angèle", backgroundImage: "/images/angele.png", date: "15 DÉCEMBRE 2020", place: "Palais des sports", city: "Lyon"},
        {id: "damso", name: "Damso", backgroundImage: "/images/damso.jpeg", date: "16 DÉCEMBRE 2020", place: "Stade Vélodrome", city: "Marseille"},
        {id: "laylow", name: "Laylow", backgroundImage: "/images/laylow.jpeg", date: "17 DÉCEMBRE 2020", place: "La grande roue", city: "Annecy"},
        {id: "rihanna", name: "Rihanna", backgroundImage: "/images/rihanna.jpeg", date: "18 DÉCEMBRE 2020", place: "Parc des Princes", city: "Paris"},
        {id: "amir", name: "Amir", backgroundImage: "/images/amir.jpeg", date: "19 DÉCEMBRE 2020", place: "Arena", city: "Nice"},
      ]
    }
  }
}
</script>

<style lang="scss">
.home {
  color: white;
  width: 100%;
  display: flex;
  flex-direction: column;
}
</style>
