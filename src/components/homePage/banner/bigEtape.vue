<template>
  <div class="bigEtape">
      <etape :number="bigEtapeData.etape1Data.number" :titre="bigEtapeData.etape1Data.titre" :text="bigEtapeData.etape1Data.text"/>
      <etape :number="bigEtapeData.etape2Data.number" :titre="bigEtapeData.etape2Data.titre" :text="bigEtapeData.etape2Data.text"/>
      <etape :number="bigEtapeData.etape3Data.number" :titre="bigEtapeData.etape3Data.titre" :text="bigEtapeData.etape3Data.text"/>

  </div>
</template>

<script lang="ts">
import etape from './etape.vue'
export default {
  name: 'bigEtape',
  props:{
    bigEtapeData: Object,
  },
  components: {
    etape,
    
  },
}
</script>
<style lang="scss">
    .bigEtape{
        display: flex;
        width: 90%;
        justify-content: space-around;
        margin: 0 auto 150px auto;
    }
</style>