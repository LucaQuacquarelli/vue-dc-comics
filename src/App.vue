<template>
  <div id="app">
    <Header/>
    <Main/>
    <Shop/>
    <Footer/>
    <FooterContact/>
  </div>
</template>

<script>
import Header from './components/Header'
import Main from './components/Main'
import Footer from './components/Footer'
import FooterContact from './components/FooterContact'
import Shop from './components/Shop'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    FooterContact,
    Shop
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700&display=swap');

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Lato', sans-serif;
  }
</style>
