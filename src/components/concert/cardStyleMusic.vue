<template>
  <div class="cardStyleMusic">
    <h3>{{titleCardStyle}}</h3>
  </div>
</template>

<script>

export default {
  name: 'cardStyleMusic',
  components: {
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
      h3{
        background: -webkit-linear-gradient(89.6deg, #211C39 -2.19%, #927BF9 102.14%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-weight: 800;
        font-size: 30px;
        font-family: 'Sora', sans-serif;
      }
    }
</style>
