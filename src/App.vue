<template>
  <div id="app">
    <!-- testata della pagina  -->
    <Header />
    <Center />
    <Footer />
    <!-- /testata della pagina  -->
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Center from "./components/Center.vue";
import Footer from "./components/Footer.vue";

export default {
  name: 'App',
  components: {
    Header,
    Center,
    Footer

  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@300;400;500;700&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Oswald', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
