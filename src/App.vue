<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
    <CopyrightSection />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import CopyrightSection from './components/CopyrightSection.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    CopyrightSection
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "~@fortawesome/fontawesome-free/css/all.css";
@import "./style/variables.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  overflow-x: hidden;
}
</style>