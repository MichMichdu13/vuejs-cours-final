<template>
  <div class="cardStyleMusic">
    <h3>{{titleCardStyle}}</h3>
    <div class="cardContainerSlide">
      <cardArtisteSlide />
      <cardArtisteSlide />
      <cardArtisteSlide />
      <cardArtisteSlide />
      <cardArtisteSlide />
    </div>
  </div>
</template>

<script>
import cardArtisteSlide from './cardArtisteSlide.vue';

export default {
  name: 'cardStyleMusic',
  components: {
    cardArtisteSlide,
  },
    props: {
      titleCardStyle: String,
  },
}
</script>
<style lang="scss">
    .cardStyleMusic{
      width: 90%;
      height: 450px;
      margin: 10px 0;
      background-color: #F3EEFF;
      border-radius: 30px;
      position: relative;
      h3{
        background: -webkit-linear-gradient(89.6deg, #211C39 -2.19%, #927BF9 102.14%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-weight: 800;
        font-size: 30px;
        font-family: 'Sora', sans-serif; 
        position: absolute;
        top: 20px;
        left: 20px;
        margin: 0;
      }
      .cardContainerSlide{
        width: 100%;
        display: flex;
        flex-wrap: nowrap;
        position: absolute;
        bottom: 25px;
        left: 35px;

      }
    }
</style>
