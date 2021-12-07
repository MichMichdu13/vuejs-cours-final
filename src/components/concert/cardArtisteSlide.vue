<template>
  <div class="cardArtisteSlide">
      <p class="dateSlide">le 20 janvier</p>
      <div class="txtbottomSlideCard">
          <p class="nameSlide">Damso</p>
          <p class="placeSlide">marseille, Velodrome </p>
      </div>
  </div>
</template>

<script>

export default {
  name: 'cardartisteSlide',
  components: {
  },
    props: {
  },
}
</script>
<style lang="scss">
    .cardArtisteSlide{
      width: 250px;
      height: 350px;
      background-color: red;
      border-radius: 20px;
      margin-right: 35px;
      position: relative;
      p{
          margin: 0;
          font-family: 'Sora', sans-serif;
      }
      .dateSlide{
          position: absolute;
          top: 10px;
          right: 10px;
      }
      .txtbottomSlideCard{
          position: absolute;
            bottom: 20px;
            left: 20px;
            .nameSlide{
                font-size: 25px;
                font-weight: 800;
            }
        }
      
    }
</style>
