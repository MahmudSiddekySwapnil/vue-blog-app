<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-list-subheader class="text-h4 justify-center" >Project</v-list-subheader>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</p>
      </v-col>
      <v-col lg="4" v-for="project in 3" :key="project">
        <v-card
            class="mx-auto"
            max-width="500px"
        >
          <v-img
              src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
              height="200px"
              cover
          ></v-img>
          <v-card-title>Web Development</v-card-title>
          <v-card-text>I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.</v-card-text>
          <v-divider class="mx-4"></v-divider>
          <v-card-actions>
            <v-btn color="success" rounded>View Details</v-btn>
            <v-spacer/>
            <v-rating
                :value="4.5"
                color="amber"
                dense
                half-increments
                readonly=""
                size="25">
            </v-rating>
          </v-card-actions>

        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>

</script>
<style scoped>

</style>