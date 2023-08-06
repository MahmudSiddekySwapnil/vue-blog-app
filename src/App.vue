<template>
  <v-app>
    <Header/>
    <v-main>
      <HeroComponent/>
      <About/>
      <Portfolio/>
      <Project/>
      <Gallery/>
      <Contact/>
      <Footer/>
    </v-main>
  </v-app>
</template>

<script>
import Header from './components/Header';
import HeroComponent from "./components/HeroComponent.vue";
import About from "./components/About.vue";
import Portfolio from "./components/Portfolio.vue";
import Project from "./components/Project.vue";
import Gallery from "./components/Gallery.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";

export default {
  name: 'App',
  components: {
    Footer,
    Contact,
    Gallery,
    Project,
    Portfolio,
    About,
    HeroComponent,
    Header,
  }
}
</script>
