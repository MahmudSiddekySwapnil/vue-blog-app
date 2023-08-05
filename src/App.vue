<template>
  <v-app>
    <Header/>
   <v-main>
      <HeroComponent/>
   </v-main>
  </v-app>
</template>

<script>
import Header from './components/Header';
import HeroComponent from "@/components/HeroComponent.vue";
export default {
  name: 'App',
  components:{
    HeroComponent,
    Header,
  }
}
</script>
