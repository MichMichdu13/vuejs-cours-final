<template>
  <div class="title2home">
    <img src="/images/boulesTitre2Home.svg" alt="bouboule">
    <h3>{{ title3 }}</h3>
  </div>
</template>

<script lang="ts">
export default {
  name: 'title',
  props: {
    title3: String,
  },
}
</script>
<style lang="scss">

.title2home{
    margin: 150px auto;
    height: 217px;
    width: 700px;
    position: relative;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Sora', sans-serif;
    h3{
        z-index: 1;
        font-size: 35px;
    }

  img{
    z-index: 0;
    position: absolute;
    left: 0;
    width: 25%;
    transform: translate(-15%, 0); 
  }
}
</style>