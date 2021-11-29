<template>
  <div class="bannerConcert">
      <titleMain :title1="bannerData.mainTitreData.titre1homeData" :title2="bannerData.mainTitreData.soustitre1homeData" />
  </div>
</template>

<script>
import titleMain from '../homePage/banner/titleMain.vue'
export default {
  name: 'bannerConcert',
  components: {
    titleMain,
  },
    props: {
    bannerData: Object,

  },
}
</script>
<style lang="scss">
    .bannerConcert{
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      background: radial-gradient(51.9% 336.54% at 51.9% 50%, #241B4D 0%, #1B1B1B 100%);
      border-radius: 0px 0px 150px 0;
    }
</style>
