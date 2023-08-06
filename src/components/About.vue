<template>
  <v-container>
    <v-row>
      <v-col lg="6">
        <v-img width="60%" src="./../assets/power.png" alt=""></v-img>
      </v-col>
      <v-col lg="6">
      <v-list-subheader class="text-md-h4">
        About Us
      </v-list-subheader>
        <p>Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source.</p>
      <v-list>
        <v-list-item>
          <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
          <v-list-item-subtitle>Contrary to popular belief, Lorem Ipsum is not simply random text.</v-list-item-subtitle>
        </v-list-item>
        <v-list-item>
          <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
          <v-list-item-subtitle>Contrary to popular belief, Lorem Ipsum is not simply random text.</v-list-item-subtitle>
        </v-list-item>
        <p>Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source.</p>
      </v-list>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name:"About"
}
</script>