<template>
  <div>
    <v-app-bar style="background-color: #2f99ee;" app dense>
      <v-container>
        <v-row align="center" no-gutters>
          <v-col sm="3" md="2" lg="2">
            <v-toolbar-title
              style="
                cursor: pointer;
                color: white;
                font-family: Montserrat;
                font-weight: bold;
              "
              @click="$router.push('/')"
              >FCOARCADENT</v-toolbar-title
            >
          </v-col>
          <v-spacer></v-spacer>
          <v-col
            v-if="$vuetify.breakpoint.smAndUp"
            style="text-align: end; font-family: Montserrat; font-weight: thin;"
            sm="9"
            md="10"
            lg="10"
          >
            <a
              class="pa-2"
              :class="{
                'mr-5': $vuetify.breakpoint.mdAndUp,
                'mr-3': $vuetify.breakpoint.sm
              }"
              style="color: white;"
              href="/about/"
              >Despre</a
            >
            <nuxt-link
              class="pa-2"
              :class="{
                'mr-5': $vuetify.breakpoint.mdAndUp,
                'mr-3': $vuetify.breakpoint.sm
              }"
              style="color: white;"
              :to="{ path: '/', hash: '#servicii' }"
            >
              Servicii Stomatologice
            </nuxt-link>
            <a
              class="pa-2"
              :class="{
                'mr-5': $vuetify.breakpoint.mdAndUp,
                'mr-3': $vuetify.breakpoint.sm
              }"
              style="color: white;"
              href="/preturi"
              >Preturi</a
            >
            <Button
              button-title="Contact"
              :has-anchor="true"
              to="/"
              anchor="#contact"
            />
          </v-col>
          <v-col v-if="$vuetify.breakpoint.xsOnly" cols="2">
            <v-app-bar-nav-icon
              @click.stop="drawer = !drawer"
            ></v-app-bar-nav-icon>
          </v-col>
          <v-navigation-drawer
            v-model="drawer"
            style="background-color: #2f99ee;"
            right
            absolute
            app
            temporary
          >
            <v-list nav dense>
              <v-list-item-group>
                <v-list-item
                  v-for="item in items"
                  :key="item.title"
                  :to="item.to"
                >
                  <v-list-item-title
                    class="text-center"
                    style="color: white; font-family: Montserrat;"
                    >{{ item.title }}</v-list-item-title
                  >
                </v-list-item>

                <!-- <v-list-item>
                  <v-list-item-title
                    class="text-center"
                    style="color: white; font-family: Montserrat;"
                    >Servicii Stomatologice</v-list-item-title
                  >
                </v-list-item>

                <v-list-item>
                  <v-list-item-title
                    class="text-center"
                    style="color: white; font-family: Montserrat;"
                    >Preturi</v-list-item-title
                  >
                </v-list-item>

                <v-list-item>
                  <v-list-item-title
                    class="text-center"
                    style="color: white; font-family: Montserrat;"
                    >Contact</v-list-item-title
                  >
                </v-list-item> -->
              </v-list-item-group> </v-list
            ><v-row>
              <v-col cols="12" class="text-center">
                <v-icon @click.stop="drawer = !drawer">mdi-close</v-icon>
              </v-col>
            </v-row>
          </v-navigation-drawer>
        </v-row>
      </v-container>
    </v-app-bar>
  </div>
  <!-- <div class="container-fluid blue flex flex-row nav-container">
    <div class="logo">
      <h1 class="h1">FCoarcaDent</h1>
    </div>
    <div class="menu">
      <ul class="nav w-100 justify-content-end">
        <li class="nav-item">
          <a class="nav-link active" href="#">Despre</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Servicii Stomatologice</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/preturi">Preturi</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </div> -->
</template>
<script>
export default {
  name: 'NavMenu',
  data: () => ({
    drawer: false,
    serviciiRoute: { name: 'HomePage', hash: '#servicii' },
    items: [
      { title: 'Despre', to: '/' },
      { title: 'Servicii Stomatologice', to: '/' },
      { title: 'Preturi', to: '/preturi' },
      { title: 'Contact', to: '/' }
    ]
  }),
  created() {
    console.log(this.$route.hash)
  },
  methods: {
    clearRoute() {
      console.log('received')
      console.log(this.$router)
    }
  }
}
</script>
<style>
/* .nav {
  height: 50px;
}

.logo h1 {
  color: white;
} */
a {
  text-decoration: none;
}
a:hover {
  text-decoration: none;
}
</style>
