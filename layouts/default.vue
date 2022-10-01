<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
          
        >
          <v-list-item-action>
            <v-tooltip bottom>
              <template v-slot:activator="{ on, attrs }">
                <v-icon
                  v-bind="attrs"
                  v-on="on">
                  {{ item.icon }}
                </v-icon>
              </template>
                <span> {{item.title}} </span>
              </v-tooltip>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        {
          icon: 'mdi-home-outline',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: ' mdi-tower-beach',
          title: 'Catapult',
          to: '/catapult'
        },
        {
          icon: 'mdi-bridge',
          title: 'Paper Bridges',
          to: '/bridge'
        },
        {
          icon: 'mdi-domino-mask',
          title: 'Mask',
          to: '/mask'
        },
        {
          icon: 'mdi-kite-outline',
          title: 'Kite',
          to: '/kite'
        },
        {
          icon: 'mdi-sofa-single-outline',
          title: 'Cardboard Funiture',
          to: '/cardboard-furniture'
        },
        {
          icon: 'mdi-shape-outline',
          title: 'Geometric Art',
          to: '/geometric-art'
        }
      ],
      miniVariant: true,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
