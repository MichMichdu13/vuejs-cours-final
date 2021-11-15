<template>
  <div class="concerts">
      <Welcome message=" lalllalalalallallalal"/>
      <Nav />
  </div>
</template>

<script>
import Welcome from '../components/Welcome.vue'
import Nav from '../components/nav-footer/Nav.vue'

export default {
  name: 'Concerts',
  components: {
    Welcome,
    Nav,
  },
}
</script>

<style lang="scss">
.concerts {
  color: white;
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>