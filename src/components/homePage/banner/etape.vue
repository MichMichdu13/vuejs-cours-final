<template>
  <div class="etape">
      <div class="number">{{number}}</div>
      <h4>{{titre}}</h4>
      <p>{{text}}</p>
  </div>
</template>

<script lang="ts">
export default {
  name: 'etape',
  props: {
    number: String,
    text: String,
    titre: String,
  },

}
</script>
<style lang="scss">
    .etape{
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 350px;
        height: 200px;
        background: rgba(0, 0, 0, 0.2);
        border-radius: 30px;
        padding: 10px;
        h4{
            margin: 0;
            font-weight: 800;
            font-size: 23px;
                background: -webkit-linear-gradient(left, #d99cf0 -2.19%, #927bf9 102.14%);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
        }
        p{
            font-weight: 200;
            font-size: 18px;
            text-align: center;
        }
        .number{
            position: absolute;
            left: 30px;
            top: -25px;
            background: linear-gradient(135deg, #D79CF1 0%, #967DF9 100%);
            border-radius: 14px;
            width: 50px;
            height: 50px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: 800;
            font-size: 25px;
        }
    }
</style>