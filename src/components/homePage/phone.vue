<template>
  <div class="phonedl">
       <div class="textPhone">
           <p class="phoneTitre">{{phoneData.phoneTiteData}}</p>
           <p class="phonetxt">{{phoneData.phonetextData}}</p>
       </div>
       <div class="phoneDLimg">
            <img src="/images/apple.png" alt="apple">
            <img src="/images/android.png" alt="android">
        </div>
    </div>
</template>



<script lang="ts">
export default {
    name: 'phone',
    props: {
    phoneData: Object,
  },
}
</script>
<style lang="scss">
  .phonedl{
    width: 600px;
    display: flex;
    flex-direction: column;
    margin: 180px auto 0 auto;
    .textPhone{
      text-align: center;
      color: black;
      .phonetxt{
        font-weight: normal;
        font-size: 20px;
        margin: 0;
      }
      .phoneTitre{
        font-family: 'Sora', sans-serif;
        font-weight: 800;
        font-size: 35px;
        margin: 10px 0;
        background: -webkit-linear-gradient(left, #d99cf0 -2.19%, #927bf9 102.14%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
    }
    .phoneDLimg{
      margin-top: 30px;
      display: flex;
      justify-content: space-evenly;
      img{
        width: 200px;
        height: 60px;
      }
    }
  }
</style>
      