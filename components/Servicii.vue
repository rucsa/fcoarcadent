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
              <v-img :src="require('./../assets/profilaxie.png')"></v-img>

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
              <v-img :src="require('./../assets/estetica.png')"></v-img>

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
              <v-img :src="require('./../assets/Endodontie.png')"></v-img>

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
              <v-img :src="require('./../assets/protetica.png')"></v-img>

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
                :src="require('./../assets/chirurgie-dentara.png')"
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
              <v-img :src="require('./../assets/parodontologie.png')"></v-img>

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
              <v-img :src="require('./../assets/ortodontie.png')"></v-img>

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
            <Button button-title="Preturi" />
          </v-col>
          <v-col cols="6" class="text-left">
            <Button button-title="Contact" />
          </v-col>
        </v-row>
      </v-card>
    </v-row>
  </v-container>
  <!-- <div class="section servicii">
    <h1 class="center">Servicii Stomatologice</h1>
    <div class="card-container">
      <Card class="profilaxie" card-title="PROFILAXIE" card-text="cardtext1" />
      <Card
        class="estetica-dentara"
        card-title="ESTETICA DENTARA"
        card-text="cardtext1"
      />
      <Card class="endodontie" card-title="ENDODONTIE" card-text="cardtext1" />
      <Card class="proteica" card-title="PROTETICA" card-text="cardtext1" />
      <Card
        class="chirurgie-dentara"
        card-title="CHIRURGIE  DENTARA"
        card-text="cardtext1"
      />
      <Card
        class="parodontologie"
        card-title="PARODONTOLOGIE"
        card-text="cardtext1"
      />
      <Card class="ortodontie" card-title="ORTODONTIE" card-text="cardtext1" />
    </div>
  </div> -->
</template>
<script>
export default {
  name: 'Servicii'
}
</script>
<style scoped>
.card-container {
  padding: 0px 15em;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.profilaxie {
  background-image: url('./../assets/profilaxie.png');
  background-size: contain;
  background-repeat: no-repeat;
}
.estetica-dentara {
  background-image: url('./../assets/estetica.png');
  background-size: contain;
  background-repeat: no-repeat;
}
.endodontie {
  background-image: url('./../assets/Endodontie.png');
  background-size: contain;
  background-repeat: no-repeat;
}
.proteica {
  background-image: url('./../assets/protetica.png');
  background-size: contain;
  background-repeat: no-repeat;
}
.chirurgie-dentara {
  background-image: url('./../assets/chirurgie-dentara.png');
  background-size: contain;
  background-repeat: no-repeat;
}
.parodontologie {
  background-image: url('./../assets/parodontologie.png');
  background-size: contain;
  background-repeat: no-repeat;
}
.ortodontie {
  background-image: url('./../assets/ortodontie.png');
  background-size: contain;
  background-repeat: no-repeat;
}
</style>
