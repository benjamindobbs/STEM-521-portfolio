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
            <v-btn href="https://www.scientificamerican.com/article/paper-bridges/" target="_blank">
                Resources
            </v-btn>
        </v-card>
        <v-card>
            <v-btn href="https://www.youtube.com/watch?v=gtUZcIDrwoo" target="_blank">
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
            This project is intended to be a design challenge. The prompt is left intentionally vague to encourage a productive struggle. Students should be encouraged to try different solutions and to work collaboritively.
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            While creating my sample project I started by examining the design requirements and the goal of the project (ISTE 1.4.b). I determined that the nature of the project really just desired a rope, not a bridge. Typically when finding solutions it is important to try a simple, and existing, solution. Students often try to reinvent the wheel and end up at a less than satisfactory solution. Research is the central pillar of good design, and simplicity is a virtue. I decided to make a braided rope and spend my time working on the support more so than the structure.  
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
          Results  
        </v-card-title>
        <v-card-text>
            My rope bridge turned to out to be fairly successful. The success of the challenge was determined by the ratio of sheets of paper used, to the mass the structure could support. I was correct in my assumption that the limiting strength would not be the paper, but the mount of the paper to the tables. 
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
            to="/mask"
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
            name: 'bridge',
            items: [
          {
            src: '/bridge/1.jpg',
          },
          {
            src: '/bridge/2.jpg',
          },
          {
            src: '/bridge/3.jpg',
          },
          {
            src: '/bridge/4.jpg',
          },
          {
            src: '/bridge/5.jpg',
          },
          {
            src: '/bridge/6.jpg',
          }
        ],
          productimages: [
          {
            src: '/bridge/6.jpg',
          }

          ]
        }
        }
    }
</script>
