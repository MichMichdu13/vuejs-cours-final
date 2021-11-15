<template>
  <div class="about">
      <Welcome message=" les femmes méprisent les bites amollies"/>
      <Nav />
  </div>
</template>

<script>
import Welcome from '../components/Welcome.vue'
import Nav from '../components/nav-footer/Nav.vue'

export default {
  name: 'About',
  components: {
    Welcome,
    Nav,
  },
}
</script>

<style lang="scss">
.about {
  color: white;
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>