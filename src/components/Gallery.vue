<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-list-subheader class="text-h4 justify-center" >Gallery</v-list-subheader>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</p>
      </v-col>
      <v-col
          v-for="n in 9"
          :key="n"
          class="d-flex child-flex"
          cols="4"
      >
        <v-img
            :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
            :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
            aspect-ratio="1"
            cover
            class="bg-grey-lighten-2"
        >
          <template v-slot:placeholder>
            <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
            >
              <v-progress-circular
                  indeterminate
                  color="grey-lighten-5"
              ></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  name:"Gallery"
}
</script>