<template>
  <div class="bigCardArtiste" :style="`background-image:url('${currentConcert.backgroundImage}')`">
      <div class="cardArtiste">
          <div class="textCard">
              <p class="date">{{currentConcert.date}}</p>
              <p class="lieu">{{currentConcert.place}}</p>
          </div>
          <button class="btnReseravtion">RÉSERVER</button>
      </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'cardArtiste',
  props: {
    topConcerts: Array,
    selectedTab: String,
    currentConcert: Object,
  },
}
</script>
<style lang="scss">
    .bigCardArtiste{
        height: 600px;
        border-radius: 0px 0px 50px 50px;
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center center;
    }

    .cardArtiste{
        height: 600px;
        background: linear-gradient(360deg, rgba(37, 26, 35, 0.98) 0%, rgba(37, 26, 35, 0) 100%);
        border-radius: 0px 0px 50px 50px;
        display: flex;
        align-items: flex-end;
        justify-content: space-between;
        z-index: 100;
        .textCard{
            margin: 20px 50px;
        }
        .btnReseravtion{
            margin: 20px 50px;
            background: linear-gradient(72.83deg, #D48AE6 0%, #9A82FC 100%);
            border-radius: 14px;
        }
        .date{
            font-family: 'Sora', sans-serif;
            font-weight: 800;
            font-size: 30px;
            margin: 0;
        }
        .lieu{
            font-family: 'Sora', sans-serif;
            font-weight: 200;
            margin: 5px 0;
        }

    }
</style>