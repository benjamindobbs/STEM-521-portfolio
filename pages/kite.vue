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
            <v-btn href="https://www.my-best-kite.com/how-to-build-kites.html" target="_blank">
                Resources
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.my-best-kite.com/flying-kites.html" target="_blank">
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
            This project is challenging. It requires students to have precise motor skills, a willingness to experiment, and the warewithal to fail repeatedly and not give up. In this project students will work with a few different materials. You need a material for the body of the kite, and the supports for the kite. You will additionally need string and a tail material. These materials can range from trashbags and dowels to mylar and carbon fiber rods.  
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            Kite building is a science. There is a time and place for student exploration and productive struggling, but this is not that. Unless you are teaching an advanced engineering course, I would say that instructions are a non-option. I used one of the basic tutorials from the provided resources page. I made mine from mylar sheet and wooden dowel. The tricky part of the build was correctly placing the mount onto the kite. The mounting point is critical for correctly balancing the kite and giving enough lift to stay in flight. 
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
            After the wind picked up a little bit I was able to get sustained flight. I was honestly impressed with the stability and consistently of the kite I made. With a very gently breeze I was able to get consistent, seemingly indefinite, flight with my little kite.
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
            to="/cardboard-furniture"
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
            name: 'kite',
            items: [
            {
            src: '/STEM-521-portfolio/kite/1.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/2.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/3.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/4.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/5.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/6.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/7.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/8.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/9.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/10.jpg',
          },
          {
            src: '/STEM-521-portfolio/kite/11.JPG',
          },
          {
            src: '/STEM-521-portfolio/kite/12.JPG',
          },
          
        ],
          processimages: [
          {
            src: '/STEM-521-portfolio/kite/11.JPG',
          },
          ],
          productimages:[
          {
            src: '/STEM-521-portfolio/kite/12.JPG',
          },
          ]
        }
        }
    }
</script>
