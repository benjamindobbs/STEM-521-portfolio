<template>
    <v-main>
        <v-carousel hide-delimiters :show-arrows="false" cycle>
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"              
            >
            
            <v-img :src=item.src contain height="100vh" width="100%"></v-img>
        </v-carousel-item>
        </v-carousel>
  <v-container>
    <v-row
    justify="space-around" class="pa-12">
        <v-card>
            <v-btn href="https://www.pinterest.com/pin/2462974774142854/" target="_blank">
                Resources
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.pinterest.com/pin/chin-colle-3d-paper-masks--92746073547691599/" target="_blank">
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
            This is a creative project. It can be combined with a creative writing prompt, or it could stem from an existing text or lore. This project is a great introduction to working with your hands and creating a product from your own idea. There are no set instructions, nor are the requirements precise. The project encourages creativity and importantly, is fun.
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            For my sample project I decided to see how far I could take the prompt on a technical level. I designed my mask using Blender, and artist 3D modeling software. After I completed my render I took the file into Mastercam and began working on toolpaths to cut my design from sign foam. I ended up with a nearly complete mask straight off the router. I took some time to add some additional details with a set of jeweler's files. I rounded over sharp edges, added additional surface imperfections and cleaned up a few of the more pitted sections from the router. Once I was happy with the form, I began painting. I employed a few prop making techniques to get my desired aesthetic. I started with a basecoat of a blue tinted silver to get a base polished steel look. I then mixed a dark mudded color and filled in all of the cracks with a fine brush. I then took a shop rag and rubbed in the color. This technique gives the a muddied look. The rag keeps more of the soil tones in the cracks while simultaneously staining the entire piece. After the muddying proccess I went back over the whole mask with a silver wash using a similar rag technique. This returned that metalic surface finish I was looking for.  
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
            My mask ended up being a different texture from my original render. I just don't have the technical skill to recreate my original style with paint. The form of the mask is spot on, and I am very happy with my final product. 
        </v-card-text>
        <v-carousel>
            <v-carousel-item
                v-for="(item,i) in productimages"
                :key="i"              
            >
            <v-img :src=item.src contain height="100vh" width="100%"> </v-img>
        </v-carousel-item>
        </v-carousel>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/kite"
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
            name: 'mask',
            items: [
            {
            src: '/STEM-521-portfolio/mask/1.JPG',
          },
          {
            src: '/STEM-521-portfolio/mask/2.png',
          },
          {
            src: '/STEM-521-portfolio/mask/3.png',
          },
          {
            src: '/STEM-521-portfolio/mask/4.PNG',
          },
        ],
        processimages: [
        {
            src: '/STEM-521-portfolio/mask/3.png',
            
          },
          {
            src: '/STEM-521-portfolio/mask/2.png',
          },
          {
            src: '/STEM-521-portfolio/mask/4.PNG',
          }
        ],
        productimages: [
        {
            src: '/STEM-521-portfolio/mask/2.png',
          },
          {
            src: '/STEM-521-portfolio/mask/1.JPG',
          }
        ]
        }
        }
    }
</script>
