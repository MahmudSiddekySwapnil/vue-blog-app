<template>
  <v-footer padless>
    <v-col lg="12">
      <v-row justify="center">
        <v-col lg="4" class="text-center">
          <v-toolbar-title>Blog App</v-toolbar-title>
          <v-card-text>
            <v-btn
                v-for="icon in icons"
                :key="icon"
                class="mx-4 black--text"
                icon>
              <v-icon size="24">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-card-text>
          <v-list-subheader>
            There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.
          </v-list-subheader>
          <v-form class="mt-4">
            <v-text-field label="Email" outlined dense></v-text-field>
            <v-btn rounded color="success">Subscribe</v-btn>
          </v-form>
        </v-col>
      </v-row>
      <div class="mt-10">
        <v-divider></v-divider>
        <v-list-subheader>
          @ Copyright Blog App. All Rights Reserved {{ new Date().getFullYear() }}
          <v-spacer/>
          <strong>Designed By Swapnil Mahmud</strong>
        </v-list-subheader>
      </div>
    </v-col>
  </v-footer>
</template>

<script>
export default{
  name:"Footer",
  data(){
    return{
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }
  }
}
</script>
<style>

</style>