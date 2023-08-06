<template>
  <v-container class="my-15">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-list-subheader class="text-h4 justify-center" >Portfolio</v-list-subheader>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</p>
      </v-col>
      <v-col lg="6">
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3747160.8545984835!2d87.702284419633!3d23.48437637265518!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x30adaaed80e18ba7%3A0xf2d28e0c4e1fc6b!2sBangladesh!5e0!3m2!1sen!2sbd!4v1691316576032!5m2!1sen!2sbd" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </v-col>
      <v-col lg="6">
        <v-form ref="form">
          <v-text-field
              v-model="contactInfo.name"
              :counter="10"
              label="Name"
              required
          ></v-text-field>

          <v-text-field
              v-model="contactInfo.email"
              :counter="10"
              label="E-mail"
              required
          ></v-text-field>

          <v-textarea
              v-model="contactInfo.massage"
              label="Massage"
          ></v-textarea>
          <v-btn color="success" class="mr-4">
            Send
          </v-btn>


        </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name:"Contact",
  data(){
    return{
      contactInfo:{}
    }
  }
}
</script>
<style scoped>

</style>