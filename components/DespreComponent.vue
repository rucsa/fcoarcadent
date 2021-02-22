<template>
  <div>
    <v-container v-if="$vuetify.breakpoint.smAndUp">
      <v-row class="pt-15 pb-14">
        <v-col
          cols="12"
          style="font-family: Montserrat; font-weight: bold; font-size: 20px;"
        >
          <h2 class="text-center">Despre noi</h2>
        </v-col>
      </v-row>
      <v-row no-gutters>
        <v-col cols="6">
          <v-img
            max-height="300px"
            max-width="600px"
            min-height="300"
            min-width="400"
            :src="require(`./../assets/img/DSC_0160.jpg`)"
          ></v-img>
        </v-col>
        <v-col cols="5" class="offset-1">
          <v-card flat tile>
            <v-card-text class="pr-10" style="color: #2d2d2d; font-size: 1rem;">
              {{ aboutUsText1 }}
              <br /><br />
              {{ aboutUsText2 }}
            </v-card-text>
            <v-card-title
              class="font-italic"
              style="font-family: Ananda; font-size: 25px; mx-1"
              >{{ specialText }}
            </v-card-title>
            <v-card-actions>
              <Button
                class="px-1"
                button-title="Servicii"
                @clicked="router.push('/about/')"
              />
              <Button
                class="px-1"
                button-title="Contact"
                @clicked="router.push('/about/')"
              />
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <v-container v-if="$vuetify.breakpoint.xsOnly">
      <!-- <v-row class="pt-15 pb-3">
        <v-col cols="12">
          <h2>Despre noi</h2>
        </v-col>
      </v-row> -->
      <v-row>
        <v-col>
          <!-- <v-card flat tile elevation="0"> -->
          <h2 class="pl-4">Despre noi</h2>
          <v-card-text style="color: #7f7f7f; font-size: 13px;">
            {{ aboutUsText1 }}
            <br /><br />

            {{ aboutUsText2 }}
          </v-card-text>
          <v-card-title style="font-family: Ananda; color: #7f7f7f;"
            >{{ specialText }}
          </v-card-title>
          <v-card-actions>
            <a
              style="
                color: #2d2d2d;
                background-color: #f2b705;
                border-radius: 25px;
                text-align: center;
                text-decoration: none;
              "
              class="px-3 pa-1"
              to="/about/"
              >Citeste mai multe</a
            >
          </v-card-actions>
          <!-- </v-card> -->
        </v-col>
      </v-row>
    </v-container>
  </div>
  <!-- <div class="container">
    <h1 class="text-center">Despre Noi</h1>
    <div class="flex">
      <div class="about-intro-img"></div>
      <div class="flex-vertical">
        <div class="about-intro-text">
          <p>
            {{ aboutUsText1 }}
          </p>
          <p>
            {{ aboutUsText2 }}
          </p>
          <blockquote>
            <h3 class="special-text">
              {{ specialText }}
            </h3>
          </blockquote>
        </div>
        <div class="flex center-items center">
          <Button button-title="Citeste mai multe" to="/about/" />
        </div>
      </div>
    </div>
  </div> -->
</template>
<script>
// import Button from '~/components/Button.vue'

export default {
  name: 'DespreComponent',
  // components: { Button },
  data() {
    return {
      aboutUsText1:
        'Misiunea unui doctor stomatolog este să readuca în viața pacienților săi placerea și dorința de a-și trăi viața la cele mai înalte standarde.',
      aboutUsText2:
        'Un zâmbet pe fața pacientului este confirmarea că ne-am îndeplinit angajamentele luate prin',
      specialText: 'Jurământul lui Hippocrate'
    }
  },
  computed: {
    owner() {
      return {}
    }
  },
  methods: {}
}
</script>

<style scoped>
.about-intro-text p {
  font-family: HindSiliguri;
  font-family: 20px;
}

.about-intro-img {
  width: 60vw;
  height: 300px;
  display: block;
  background-image: url('./../assets/img/DSC_0160.jpg');
  background-size: cover;
  background-repeat: no-repeat;
}

.about-intro-text {
  padding: 1vh 5vw;
}

@media screen and (max-width: 750px) {
  .about-intro-img {
    display: none;
  }
}
</style>
