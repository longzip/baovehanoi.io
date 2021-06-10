<template>
  <div>
    <navbar-component></navbar-component>
    <Nuxt />
    <footer-component></footer-component>
  </div>
</template>
<script>
import NavbarComponent from '../components/Navbar.vue'
import FooterComponent from '../components/Footer.vue'
export default {
  components: {
    NavbarComponent,
    FooterComponent,
  },
}
</script>
