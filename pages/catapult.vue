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
            <v-btn href="https://frugalfun4boys.com/how-to-build-water-balloon-launcher/" target="_blank">
                Resources
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.instructables.com/Water-Balloon-Launcher/" target="_blank">
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
            This project is incredibly enagaging and surprisingly simple. The project consists of constructing a free standing structure capable of launching water balloons using an elastic slingshot. The structure should be made from dimensional lumber, but the size of the final project is entirely up to you.
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            Students should begin by researching the project, planning the entire structure, and creating a cut list. Students would then make their cuts and assemble their projects. My group started by working in Solidworks to determine the proper angles to maximize our distance. We determined the waterballoon should release at a 45 degree angle, and that the elastic could be pulled to a maximum distance of 10 feet. With those two pieces of information we were able to create a rough design of our project. We made sure to add ample support in the form of cross bracing. We specifically chose to make an 'X' shape with our supports to ensure the balloons had a valid path to travel upon release without hitting the supports.
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
            Our structure was very successful. We had very few missfires, and the design was incredibly consistent. The standard deviation of our shots was less than 40ft and we averaged 280ft distance per shot with a 24 m/s launch velocity. 
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
            to="/bridge"
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
            name: 'catapult',
            items: [
            {
            src: '/catapult/1.jpg',
          },
          {
            src: '/catapult/2.jpg',
          },
          {
            src: '/catapult/3.jpg',
          },
          {
            src: '/catapult/4.jpg',
          },
          {
            src: '/catapult/5.jpg',
          },
          {
            src: '/catapult/6.jpg',
          },
          {
            src: '/catapult/7.jpg',
          },
          {
            src: '/catapult/8.jpg',
          },
          {
            src: '/catapult/9.jpg',
          },
          {
            src: '/catapult/10.jpg',
          },
          {
            src: '/catapult/11.jpg',
          },
          {
            src: '/catapult/12.jpg',
          },
          {
            src: '/catapult/13.jpg',
          }
          
        ],
        processimages: [
        {
            src: '/catapult/13.jpg',
          },
          {
            src: '/catapult/8.jpg',
          },
          {
            src: '/catapult/2.jpg',
          },
          {
            src: '/catapult/3.jpg',
          },
          {
            src: '/catapult/7.jpg',
          },
          {
            src: '/catapult/5.jpg',
          }
        ],
        productimages: [
            {
            src: '/catapult/10.jpg',
          },
          {
            src: '/catapult/9.jpg',
          },
          {
            src: '/catapult/6.jpg',
          },

        ]
        }
        }
    }
</script>
