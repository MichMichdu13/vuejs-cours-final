<template>
  <nav class="footer">
    <div class="boxLogofooter">
      <router-link to="/" class="buukLogofooter">buuk</router-link>
    </div>
    <a href="" class="lienfooter">Conditions de ventes</a>
    <a href="" class="lienfooter">Mentions légales</a>
    <p>Un problème ? +33 4 50 44 56 03</p>
  </nav>
</template>

<script lang="ts">
export default {
  name: 'footer',
}
</script>

<style lang="scss">

.footer {
    margin-top: 100px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  width: 100%;
  height: 100px;
  font-size: 25px;

  p{
    margin: 0 40px;
    font-weight: 600;
    font-size: 16px;
    font-family: 'Sora', sans-serif;
    text-align: right;
    color: black;
  }
  .buukLogofooter{
    font-weight: 800;
    font-size: 35px;
    text-decoration: none;
    font-family: 'Sora', sans-serif;
    background: -webkit-linear-gradient(left, #d99cf0 -2.19%, #927bf9 102.14%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .boxLogofooter{
    position:absolute;
    left:0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100px;
    width: 181px;
  }
    .lienfooter {
      margin: 0 40px;
      font-weight: 300;
      font-size: 16px;
      text-decoration: none;
      font-family: 'Sora', sans-serif;
      color: black;
    }
  }

</style>