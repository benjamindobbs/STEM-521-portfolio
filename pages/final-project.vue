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
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </v-card-text>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
        Process
        </v-card-title>
        <v-card-text>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </v-card-text>
        <v-carousel>
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"
                :src="item.src"
            ></v-carousel-item>
        </v-carousel>
    </v-card>
    <v-card class="ma-6">
        <v-card-title>
          Results  
        </v-card-title>
        <v-card-text>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </v-card-text>
        <v-carousel>
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"
                :src="item.src"
            ></v-carousel-item>
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
            name: 'final-project',
            items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          }
        ]
        }
        }
    }
</script>
