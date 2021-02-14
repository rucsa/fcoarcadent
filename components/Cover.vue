<template>
  <div>
    <v-container class="pa-0 ma-0" fluid>
      <v-row>
        <v-col>
          <v-card flat tile>
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
                    cols="3"
                    sm="5"
                    md="4"
                    lg="3"
                    style="
                      background-color: #05aff2;
                      border-top-right-radius: 5px;
                      border-bottom-right-radius: 5px;
                    "
                  >
                    <h2 style="text-align: end; font-size: 22px;">
                      {{ title }}
                    </h2>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="3" sm="5" md="4" lg="3">
                    <h2
                      class="font-italic"
                      style="
                        color: #05aff2;
                        font-family: Ananda;
                        text-align: end;
                      "
                    >
                      {{ title2 }}
                    </h2>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col
                    cols="3"
                    sm="5"
                    md="4"
                    lg="3"
                    style="
                      background-color: #05aff2;
                      border-top-right-radius: 5px;
                      border-bottom-right-radius: 5px;
                    "
                  >
                    <h4 style="text-align: end; font-size: 20px;">
                      <span class="font-weight-medium">Lucrăm cu oameni </span
                      ><br /><span class="font-weight-bold"
                        >și pentru oameni</span
                      >
                    </h4>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="3" class="offset-2">
                    <a
                      style="
                        background-color: #f2b705;
                        border-radius: 5px;
                        text-align: center;
                      "
                      class="px-3 pa-1"
                      href="#"
                      >Vezi preturi</a
                    >
                  </v-col>
                </v-row>
              </v-card-text>
              <!-- </v-col>
            </v-row> -->
              <!-- </v-container> -->
            </v-img>
          </v-card>
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
</style>
