<template>
    <v-container class="my-15">
      <v-row justify="center">
        <v-col lg="12" class="text-center">
          <v-list-subheader class="text-h4 justify-center" >Portfolio</v-list-subheader>
          <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</p>
        </v-col>
        <v-col lg="12">
          <div class="text-center">
            <v-chip @click="activePortfolio = 'webapp'" :color="activePortfolio === 'webapp'? 'success':''" class="mx-5">Web App</v-chip>
            <v-chip @click="activePortfolio = 'mobileapp'" :color="activePortfolio === 'mobileapp'? 'success':''" class="mx-5">Mobile App</v-chip>
            <v-chip @click="activePortfolio = 'desktopapp'" :color="activePortfolio === 'desktopapp' ? 'success':''" class="mx-5">Desktop App</v-chip>
          </div>
        </v-col>
        <slot v-if="activePortfolio === 'webapp'">
          <v-col lg="3" v-for="(web,webindex) in webApps" :key="webindex">
            <v-card>
              <v-img
                  :src="web.image"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px">
                <v-card-title color="white"> {{web.title}}</v-card-title>
              </v-img>
            </v-card>
          </v-col>
        </slot>


        <slot v-if="activePortfolio === 'mobileapp'">
          <v-col lg="3" v-for="(mobile,mobileappindex) in mobileapps" :key="mobileappindex">
            <v-card>
              <v-img
                  :src="mobile.image"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px">
                <v-card-title color="white"> {{mobile.title}}</v-card-title>
              </v-img>
            </v-card>
          </v-col>
        </slot>
      </v-row>
    </v-container>
</template>

<script>
  export default {
    name: "Portfolio",
    data(){
      return{
        activePortfolio:'webapp',
        webApps:[
          {title:'web App 1', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'web App 2', image:'https://img.freepik.com/free-vector/demo-concept-illustration_114360-7612.jpg?size=626&ext=jpg'},
          {title:'web App 3', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'web App 4', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'web App 5', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'web App 6', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'}

        ],
        mobileapps:[
          {title:'mobile App 1', image:'https://img.freepik.com/free-vector/features-overview-concept-illustration_114360-1481.jpg?size=626&ext=jpg'},
          {title:'mobile App 2', image:'https://img.freepik.com/free-vector/demo-concept-illustration_114360-7612.jpg?size=626&ext=jpg'},
          {title:'mobile App 3', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'mobile App 4', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'mobile App 5', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'},
          {title:'mobile App 6', image:'https://img.freepik.com/free-vector/tiny-business-people-with-digital-devices-testing-demo-software-beta-testing-new-product-testing-presale-user-experience-concept-bright-vibrant-violet-isolated-illustration_335657-1024.jpg?w=740&t=st=1691307760~exp=1691308360~hmac=4a2e9f75466e698bc76ccad92531bd59964761a604053634fa8be30a338318b5'}
        ]
      }
    }
  }
</script>
<style scoped>

</style>