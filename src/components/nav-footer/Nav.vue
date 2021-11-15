<template>
  <nav class="nav">
    <div class="boxLogo">
      <router-link to="/" id="buukLogo">buuk</router-link>
    </div>
    <div class="box">
      <router-link to="/" >Accueil</router-link>
    </div>
    <div class="box">
      <router-link to="/concerts">Tous les concerts</router-link>
    </div>
    <div class="box">
      <router-link to="/about">Mes réservations</router-link>
    </div>
    <p>+33 4 50 67 33 22</p>
  </nav>
</template>

<script lang="ts">
export default {
  name: 'Nav',
}
</script>

<style lang="scss">


.nav {

  position: relative;
  display: flex;
  align-items: center;
  width: 100%;
  height: 75px;
  font-size: 25px;
  border-bottom: 1px solid rgb(89, 89, 89);
  background: radial-gradient(51.9% 336.54% at 51.9% 50%, #241B4D 0%, #1B1B1B 100%);;
  p{
    color: white;
    position: absolute;
    right: 20px;
    margin: 0;
    font-weight: 300;
    font-size: 20px;
    font-family: 'Sora', sans-serif;
    text-align: right;
  }
  #buukLogo{
    font-weight: 800;
    font-size: 30px;
    text-decoration: none;
    font-family: 'Sora', sans-serif;
    color: white;
  }
  .boxLogo{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 74px;
    width: 181px;
    border-right: 1px solid rgb(89, 89, 89);
  }
  .box{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 74px;
    &:hover{
      border-bottom: 2px solid #D48AE6;
      a{
        color: #D48AE6;
      }
    }
    a {
      margin: 0 40px;
      font-weight: 300;
      font-size: 20px;
      text-decoration: none;
      font-family: 'Sora', sans-serif;
      color: white;
    }
  }
}
</style>