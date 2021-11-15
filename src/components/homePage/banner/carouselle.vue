<template>
  <div class="caroucelle">
    <button 
      v-for="concert in topConcerts" 
      @click="updateSelectedTab(concert.id)" :key="concert.id"  :class="{ 'btnArtisteActif': selectedTab === concert.id }"
    >
      {{ concert.name }}
    </button>
    <cardArtiste v-model:currentConcert="topConcerts.filter(concert => concert.id === selectedTab)[0]"/>
  </div>
</template>


<script lang="ts">
import cardArtiste from './cardArtiste.vue'
export default {
  name: 'artistes',
  data(){
    return{
      selectedTab: "angele",

    }
  },
  props: {
    topConcerts: Array,
  },
    components: {
    cardArtiste,
  },
    methods: {
      updateSelectedTab(tabId) {
          this.selectedTab = tabId
      }
    }
}
</script>



<style lang="scss">
    .caroucelle{
        width: 90%;
        margin: 0 auto;
        button{
            height: 70px;
            width: 20%;
            font-family: 'Sora', sans-serif;
            font-weight: 800;
            font-size: 20px;
            color: white;
            border: none;
            background: none;
            // border-right: 1px solid #595959;
        }
        .btnArtisteActif{
            background: linear-gradient(75.5deg, #DA8BE3 0%, #9681FD 95.43%);
            border-radius: 30px 30px 0px 0px;
        }
        // #lastbutton{
        //     border: none;
        // }
    }
</style>