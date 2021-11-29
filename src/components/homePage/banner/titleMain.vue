<template>
  <div class="titleMainHome">
    <img src="/images/boulesTitreHome.svg" alt="bouboule">
    <h1>{{ title1 }}</h1>
    <h3>{{ title2 }}</h3>
  </div>
</template>

<script lang="ts">
export default {
  name: 'title',
  props: {
    title1: String,
    title2: String,
  },
}
</script>
<style lang="scss">

.titleMainHome {
  margin: 200px 0;
  height: 217px;
  position: relative;
  color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-family: 'Sora', sans-serif;
  h1{
    font-weight: 800;
    font-size: 50px;
    margin: 0;
    z-index: 1;
  }
  h3{
    font-size: 40px;
    background: -webkit-linear-gradient(left, #d99cf0 -2.19%, #927bf9 102.14%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin: 0;
    z-index: 1;
    }
  img{
    z-index: 0;
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%); 
  }
}
</style>