<template>
  <div id="app">
    <Header msg="navigation"></Header>
    <Home msg="home"></Home>
    <About msg="about"></About>
    <Pricing msg="pricing"></Pricing>
    <Testimonials msg="Testimonials"></Testimonials>
    <Download msg="download"></Download>
    <Footer msg="about"></Footer>
    
    <div id="preloader" style="display: none;"> 
      <div id="loader"></div>
    </div>  
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Home from './components/Home.vue';
import About from './components/About.vue';
import Download from './components/Download.vue';
import Pricing from './components/Pricing.vue';
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';
import Testimonials from './components/Testimonials.vue';

@Component({
  components: {
    Home,
    About,
    Download,
    Pricing,
    Footer,
    Header,
    Testimonials,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
@import 'src/assets/css/base.scss';
@import 'src/assets/css/vendor.scss';
@import 'src/assets/css/main.scss';
</style> 
