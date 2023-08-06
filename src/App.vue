<template>
  <v-app>
    <Header/>
   <v-main>
      <HeroComponent/>
       <About/>
     <Portfolio/>
   </v-main>
  </v-app>
</template>

<script>
import Header from './components/Header';
import HeroComponent from "./components/HeroComponent.vue";
import About from "./components/About.vue";
import Portfolio from "./components/Portfolio.vue";
export default {
  name: 'App',
  components:{
    Portfolio,
    About,
    HeroComponent,
    Header,
  }
}
</script>
