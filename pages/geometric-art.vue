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
            <v-btn href="https://www.weareteachers.com/10-geometric-art-explorations/" target="_blank">
                Resources
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.pinterest.com/hmahmoudian/geometric-art/" target="_blank">
                Exemplar
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="http://www.corestandards.org/Math/Content/HSG/GPE/" target="_blank">
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
            This project is an intersection between geometry and art. The direct connection to standards fall into math and art (see standards above). For our purposes, this activity is a hands on method for teaching area and volume, but could easily be modified to include perimiter or other geometric equations.
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            My project was meant to be a stained glass inpired depiction of a regal king. My process began in Adobe Illustrator, a digital vector based art software. I chose Illustrator because I specifically wanted to work in vector to have an easier time matching the geometric tropes commonly assosiated with stained glass. This project does not require any software, and designs could easily be rendered on graph paper or simply done in real time. I would steer students away from overlycomplex patterns for this project so that they don't get frustrated when they need to start doing the math. I used my illustrator file to lasercut cardboard to the exact shape I needed. This could be done with a box cuttuer, or scissors for a more low-tech approach. Once my design was created, I began measuring and solving the area of each individual shape.  
        </v-card-text>
        <v-carousel>
            <v-carousel-item
                v-for="(item,i) in processimages"
                :key="i"              
            >
            <v-img :src=item.src contain height="100vh" width="100%"> </v-img>
        </v-carousel-item>
        </v-carousel>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
          Results  
        </v-card-title>
        <v-card-text>
            My final product looked how I envisioned it, but I certainly regretted the complexity as I was solving the math. The repetitive nature of the equations, and even just the monotony of breaking each shape down to a solvable equation was hard to get through, even as an alleged patient adult. I can only imagine getting a 14 year old to solve the area of 35 triangles.
        </v-card-text>
        <v-carousel>
            <v-carousel-item
                v-for="(item,i) in productimages"
                :key="i"              
            >
            <v-img :src=item.src contain height="100vh" width="100%"> </v-img>
        </v-carousel-item>
        </v-carousel>
    </v-card>
  </v-container>
    </v-main>
</template>
<script>
export default {
    data () {
        return {
            name: 'geometric-art',
            items: [
          {
            src: '/STEM-521-portfolio/geometric-art/1.JPG',
          },
          {
            src: '/STEM-521-portfolio/geometric-art/2.JPG',
          },
          {
            src: '/STEM-521-portfolio/geometric-art/3.png',
          }
        ],
        processimages: [
            {
            src: '/STEM-521-portfolio/geometric-art/3.png',
          },
          {
            src: '/STEM-521-portfolio/geometric-art/1.JPG',
          },
        ],
        productimages: [
        {
            src: '/STEM-521-portfolio/geometric-art/1.JPG',
          },
          {
            src: '/STEM-521-portfolio/geometric-art/2.JPG',
          },
        ]
        }
        }
    }
</script>
