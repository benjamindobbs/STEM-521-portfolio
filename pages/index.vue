<template>
  <v-main>
      <v-card>
        <v-card-title class="headline">
          STEM-521 Portfolio
        </v-card-title>
        <v-card-text>
          This document contains a repository of resources generated throughout the TE-531 course. To look at a project choose one from the sidebar or press 'continue'
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/catapult"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
      <v-carousel hide-delimiters :show-arrows="false" cycle>
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"              
            >
            <v-img :src=item.src contain height="80vh" width="100%"> </v-img>
        </v-carousel-item>
  </v-carousel>
    </v-main>
</template>

<script>
export default { 
   data () {
      return {
        name: 'IndexPage',
        items: [
          {
            src: "/home/2.jpg"
          },
          {
            src: "/home/3.jpg"
          },
          {
            src: "/home/4.jpg"
          },
          {
            src: "/home/5.jpg"
          },
          {
            src: "/home/7.jpg"
          },
          {
            src: "/home/11.jpg"
          },
          {
            src: "/home/12.JPG"
          },
        ]    
      }
   }
}
</script>
