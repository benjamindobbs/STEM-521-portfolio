<template>
    <v-main>
        <v-carousel hide-delimiters :show-arrows="false" cycle>
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"              
            >
            <v-img :src=item.src contain height="100vh" width="100%"> </v-img>
        </v-carousel-item>
        </v-carousel>
  <v-container>
    <v-row
    justify="space-around" class="pa-12">
        <v-card>
            <v-btn href="https://www.thespruce.com/cardboard-furniture-designs-3017215" target="_blank">
                Resources
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.homedit.com/cardboard-furniture/" target="_blank">
                Exemplar
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.iste.org/standards/iste-standards-for-students" target="_blank">
                Standards
            </v-btn>
        </v-card>
    </v-row>
    <v-spacer></v-spacer>
    <v-card class="ma-6">
        <v-card-title>
            Description
        </v-card-title>
        <v-card-text>
            Cardboard furniture is an accessible and inexpensive design challenge. The challenge in itself is to create a piece of furniture entirely from cardboard and adhesives that is strong enough to support the creators weight. 
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            My sample project was more of an art piece than it was a practical peice of furniture. I started with a rough sketched idea, that I then brought into CAD to calculate the required measurement. I made an initial attempt of the project, but was not satisfied with the result. Afterwards, I made a second attempt of the project and simplified the design significantly. I still ran into several issues, mostly with tolerances... But eventually ended with a product that was vaguely representative of my initial design.
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
          Results  
        </v-card-title>
        <v-card-text>
            The final product was certainly less than satisfactory, but by the metrics of the project, it was successful. Were I to do the project again, I would add additional clearance on the intersecting regions of the design.
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/geometric-art"
          >
            Continue
          </v-btn>
        </v-card-actions>
    </v-card>
  </v-container>
    </v-main>
</template>
<script>
export default {
    data () {
        return {
            name: 'cardboard-furniture',
            items: [
          {
            src: '/STEM-521-portfolio/cardboard-furniture/1.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/2.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/3.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/4.JPG',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/5.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/6.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/7.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/8.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/9.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/10.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/11.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/12.jpg',
          },
          {
            src: '/STEM-521-portfolio/cardboard-furniture/13.jpg',
          }
        ],
        }
        }
    }
</script>
