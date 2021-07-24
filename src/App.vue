<template>
  <Header></Header>
  <Body></Body>
  <Footer></Footer>
  <credits></credits>
  <modal></modal>
</template>

<script>
import Header from './components/HeaderPage.vue'
import Body from './components/BodyPage.vue'
import Footer from './components/FooterPage.vue'
import Credits from './components/CreditsPage.vue'
import Modal from './components/Modal.vue'




export default {
  name: 'App',
  components: {
    Header,
    Body,
    Footer,
    Credits,
    Modal,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
