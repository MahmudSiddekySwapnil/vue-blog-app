<template>
   <v-container class="pt-15">
     <v-row>
       <v-col lg="6">
         <h2 class="intro-text">Welcome to our Vuetify App</h2>
         <p class="description">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
         <v-btn color="success" class="white--text mr-10" rounded>Get Started</v-btn>
         <v-btn color="indigo" class="white--text" rounded>
           <v-icon>mdi-play-circle</v-icon>Watch Video
         </v-btn>
       </v-col>
       <v-col lg="6">
         <v-img width="80%" src="./../assets/Power-Plant.png" alt=""></v-img>
       </v-col>
     </v-row>
   </v-container>
</template>

<script setup>

</script>
<style scoped>
h2.intro-text{
  font-size: 90px;
  font-weight: bold;
  font-family: cursive;
  color:#444;
}
p.description{
  font-size: 20px;
  font-family: cursive;
  margin: 32px 0px;
  color: #444444ba;
}
</style>