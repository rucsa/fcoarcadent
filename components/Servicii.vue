<template>
  <v-container class="my-12" fluid style="background-color: #2f99ee;">
    <v-row class="mb-12 pt-14">
      <v-col
        style="font-family: Montserrat; font-weight: bold; font-size: 20px;"
      >
        <h2 class="text-center white--text">
          Servicii
        </h2>
      </v-col>
    </v-row>
    <v-row justify="center">
      <v-card flat tile max-width="700px" color="transparent">
        <v-row justify="center">
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img :src="require('~/assets/img/profilaxie.png')"></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  PROFILAXIE
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img :src="require('~/assets/img/estetica.png')"></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  ESTETICA DENTARA
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img :src="require('~/assets/img/Endodontie.png')"></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  ENDODONTIE
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img :src="require('~/assets/img/protetica.png')"></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  PROTETICA
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img
                :src="require('~/assets/img/chirurgie-dentara.png')"
              ></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  CHIRURGIE DENTARA
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img :src="require('~/assets/img/parodontologie.png')"></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  PARODONTOLOGIE
                </div>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="3" lg="3">
            <v-card class="mx-auto" max-width="200" tile>
              <v-img :src="require('~/assets/img/ortodontie.png')"></v-img>

              <v-card-text>
                <div
                  class="text-center"
                  style="color: #05aff2; font-size: 12px;"
                >
                  ORTODONTIE
                </div>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
        <v-row class="py-5 mb-5">
          <v-col cols="6" class="text-right">
            <Button
              :has-anchor="false"
              button-title="Preturi"
              path="/preturi"
            />
          </v-col>
          <v-col cols="6" class="text-left">
            <Button
              button-title="Contact"
              :has-anchor="true"
              path="/"
              anchor="#contact"
            />
          </v-col>
        </v-row>
      </v-card>
    </v-row>
  </v-container>
</template>
<script>
export default {
  name: 'Servicii'
}
</script>
<style scoped></style>
