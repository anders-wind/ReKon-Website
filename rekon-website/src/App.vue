<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Navigation msg="navigation"></Navigation>
    <Home msg="home"></Home>
    <About msg="about"></About>
    <Pricing msg="pricing"></Pricing>
    <Testimonials msg="Testimonials"></Testimonials>
    <Download msg="download"></Download>
    <Footer msg="about"></Footer>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Home from './components/Home.vue';
import About from './components/About.vue';
import Download from './components/Download.vue';
import Pricing from './components/Pricing.vue';
import Footer from './components/Footer.vue';
import Navigation from './components/Navigation.vue';
import Testimonials from './components/Testimonials.vue';

@Component({
  components: {
    Home,
    About,
    Download,
    Pricing,
    Footer,
    Navigation,
    Testimonials
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
