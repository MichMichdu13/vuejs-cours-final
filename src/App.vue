<template>
  <Nav />
  <router-view/>
  <Footer />
</template>
<script>
import Nav from './components/nav-footer/Nav.vue'
import Footer from './components/nav-footer/Footer.vue'
  export default {
    setup() {
      return {};
    },
    components:{
      Nav,
      Footer,
    }
  };
</script>