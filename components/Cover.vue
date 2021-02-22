<template>
  <div>
    <v-container class="pa-0 ma-0" fluid>
      <v-row>
        <v-col>
          <v-card v-if="$vuetify.breakpoint.smAndUp" flat tile>
            <v-img max-height="702px" :src="require(`./../assets/LPPhoto.png`)">
              <!-- <v-container
              class="pa-0 red align-center"
              style="margin-top: 200px;"
            > -->
              <!-- <v-row align="center" style="margin-top: 200px;">
              <v-col cols="12"> -->
              <v-card-text class="white--text pl-0" style="margin-top: 200px;">
                <v-row>
                  <v-col
                    cols="4"
                    sm="7"
                    md="6"
                    lg="5"
                    style="
                      background-color: #2f99ee;
                      border-top-right-radius: 5px;
                      border-bottom-right-radius: 5px;
                      font-family: Montserrat;
                      font-weight: bold;
                    "
                  >
                    <h2
                      style="text-align: end; font-size: 30px;"
                      class="py-2 pr-1"
                    >
                      {{ title }}
                    </h2>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col
                    cols="4"
                    sm="7"
                    md="6"
                    lg="5"
                    style="
                      background: rgba(255, 255, 255, 0.5);
                      border-top-right-radius: 5px;
                      border-bottom-right-radius: 5px;
                    "
                  >
                    <h2
                      class="font-italic pr-16"
                      style="
                        color: #2f99ee;
                        font-family: Ananda;
                        text-align: end;
                        font-size: 35px;
                        padding-top: 0.7em;
                        padding-bottom: 0.5rem;
                      "
                    >
                      {{ title2 }}
                    </h2>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col
                    cols="4"
                    sm="6"
                    md="5"
                    lg="4"
                    style="
                      background-color: #2f99ee;
                      border-top-right-radius: 5px;
                      border-bottom-right-radius: 5px;
                      font-family: Montserrat;
                    "
                  >
                    <h4 style="text-align: end; font-size: 20px;">
                      <span class="font-weight-medium pr-9"
                        >Lucrăm cu oameni </span
                      ><br /><span style="font-weight: bold;"
                        >și pentru oameni</span
                      >
                    </h4>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="4" sm="6" md="5" lg="4" class="mx-16 mt-8">
                    <v-spacer />
                    <v-spacer />
                    <Button button-title="Afla mai multe" @clicked="toAbout" />
                    <Button button-title="Prețuri" />
                  </v-col>
                </v-row>
              </v-card-text>
              <!-- </v-col>
            </v-row> -->
              <!-- </v-container> -->
            </v-img>
          </v-card>
          <v-container
            v-if="$vuetify.breakpoint.xsOnly"
            fluid
            class="px-0"
            style="background-color: #e3e3e3;"
          >
            <v-row>
              <v-col cols="12">
                <h2
                  class="font-weight-medium text-center"
                  style="font-size: 22px;"
                >
                  {{ title }}
                </h2>
              </v-col>
              <!-- </v-row>
            <v-row> -->
              <v-col cols="12">
                <h1
                  class="font-italic text-center"
                  style="background-color: #2f99ee; font-family: Ananda;"
                >
                  {{ title2 }}
                </h1>
              </v-col>
              <!-- </v-row>
            <v-row> -->
              <v-col cols="12">
                <h4
                  style="font-size: 20px;"
                  class="font-weight-medium text-center"
                >
                  <span>Lucrăm cu oameni </span><br /><span
                    >și pentru oameni</span
                  >
                </h4>
              </v-col>
            </v-row>
          </v-container>
        </v-col>
      </v-row>
    </v-container>
  </div>

  <!-- <div class="cover">
    <div class="cover-content">
      <div class="cover-text">
        <h1 class="h1 anada">{{ title }}</h1>
        <h1 class="h1">
          <span class="monser">{{ title2 }}</span>
        </h1>
        <h3 class="h3">
          <span class="text-medium">Lucrăm cu oameni </span><br /><span
            class="text-bold"
            >și pentru oameni</span
          >
        </h3>
      </div>
      <div class="cover-buttons flex center-items center">
        <Button button-title="Despre noi" to="#" />
        <Button button-title="Contact" to="#" />
      </div>
    </div>
  </div> -->
</template>
<script>
// import Button from '~/components/Button.vue'

export default {
  name: 'Cover',
  // components: { Button },
  data() {
    return {
      title: 'Cabinet Stomatologic',
      title2: 'dr. Filofteia Coarcă'
    }
  },
  methods: {
    toAbout() {
      this.$router.push('/about')
    }
  }
}
</script>
<style scoped>
/* h1,
.anada {
  font-family: 'Ananda';
}

h2,
.monser {
  font-family: 'Montserrat';
}

.cover {
  background-image: url('./../assets/LPPhoto.png');
  background-repeat: no-repeat;
  background-size: contain;
  max-width: 100vw;
  height: 702px;
  border: 1px solid black;
}
.cover-content {
  position: relative;
  top: 10em;
  left: 6em;
  width: 25em;
  height: 20em;
  border: 1px solid black;
} */

a:hover {
  text-decoration: none;
}
</style>
