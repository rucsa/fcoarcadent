<template>
  <v-container class="mt-12">
    <v-row>
      <v-col cols="12" sm="6">
        <v-card flat tile>
          <v-card-text style="color: black; font-size: 15px;">
            <strong>Medic titular: </strong>{{ name }} <br /><br />

            <strong>Grad medical: </strong>{{ grad }} <br /><br />
            <strong>Experiență: </strong>{{ experienta }} <br /><br />
            <strong>Perfecționare profesională:</strong>{{ perfectionare }}
            <br /><br />
            <strong>Atitudine: </strong>{{ atitudine }} <br /><br />
            <div
              class="font-italic"
              style="color: #05aff2; font-family: Italianno; font-size: 25px;"
            >
              {{ specialtext }}
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col v-if="$vuetify.breakpoint.smAndUp" cols="5" class="offset-md-1">
        <v-img
          max-height="300px"
          max-width="600px"
          min-height="300"
          min-width="400"
          :src="require(`./../assets/DSC_0206.jpg`)"
        ></v-img>
      </v-col>
    </v-row>

    <v-row justify="center" align="center" class="py-16 my-16">
      <v-col cols="12" sm="4" md="3" lg="3">
        <v-card class="mx-auto" color="#05AFF2" width="250" height="250">
          <v-card-text>
            <v-img
              class="mt-2"
              style="display: block; margin-left: auto; margin-right: auto;"
              width="50"
              height="50"
              :src="require(`./../assets/icons/1.png`)"
            ></v-img>
            <div class="text-center white--text mt-4" style="font-size: 12px;">
              Profesionalismul și dedicația personalului medical
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="4" md="3" lg="3">
        <v-card class="mx-auto" color="#05AFF2" width="250" height="250">
          <v-card-text>
            <v-img
              class="mt-2"
              style="display: block; margin-left: auto; margin-right: auto;"
              width="50"
              height="50"
              :src="require(`./../assets/icons/2.png`)"
            ></v-img>
            <p class="text-center white--text mt-4" style="font-size: 12px;">
              Aparatură medicală stomatologică de ultimă generație
            </p>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="4" md="3" lg="3">
        <v-card class="mx-auto" color="#05AFF2" width="250" height="250">
          <v-card-text>
            <v-img
              class="mt-2"
              style="display: block; margin-left: auto; margin-right: auto;"
              width="50"
              height="50"
              :src="require(`./../assets/icons/3.png`)"
            ></v-img>
            <p class="text-center white--text mt-4" style="font-size: 12px;">
              Tehnici medicale stomatologice inovatoare
            </p>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="4" md="3" lg="3">
        <v-card class="mx-auto" color="#05AFF2" width="250" height="250">
          <v-card-text>
            <v-img
              class="mt-2"
              style="display: block; margin-left: auto; margin-right: auto;"
              width="50"
              height="50"
              :src="require(`./../assets/icons/4.png`)"
            ></v-img>
            <p class="text-center white--text mt-4" style="font-size: 12px;">
              Adresabilitate maximă corespunzătoare cerințelor pacienților
            </p>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  <!-- <div class="">
    <div class="">
      <div class="">
        <p>Medic titular: {{ name }}</p>
        <p>Grad medical: {{ grad }}</p>
        <p>Experiență: {{ experienta }}</p>
        <p>Perfecționare profesională: {{ perfectionare }}</p>
        <p>Atitudine: {{ atitudine }}</p>
        <h3 class="">{{ specialtext }}</h3>
      </div>
      <div class="about-intro-img"></div>
    </div>
    <div>
      <div class="">
        <div class="">
          <IconCard
            imagesrc="~/assets/icons/1.png"
            card-text="Profesionalismul si dedicatia personalului medical"
          />
          <IconCard
            imagesrc="~/assets/icons/2.png"
            card-text="Aparatura medicala stomatologica de ultima generatie"
          />
          <IconCard
            imagesrc="~/assets/icons/3.png"
            card-text="Tehnici medicale stomatologice inovatoare"
          />
          <IconCard
            imagesrc="~/assets/icons/4.png"
            card-text="Adresabilitate maxima corespunzatoare cerințelor pacienților"
          />
        </div>
      </div>
    </div>
  </div> -->
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      name: 'Coarcă Filofteia',
      grad: 'Medic stomatolog specialist',
      experienta:
        '33 ani vechime și peste 10.000 de pacienți tratati cu succes',
      perfectionare:
        'Continuă prin participare la congrese, simpozioane, workshopuri, cursuri de perfecționare în stomatologie',
      atitudine: 'Hotărîre, perseverență, apropiat și înțelegător cu pacienții',
      specialtext: 'Apreciată de micii pacienti'
    }
  },
  computed: {
    owner() {
      return {
        name: 'Filofteia Coarca'
      }
    }
  },
  methods: {}
}
</script>

<style scoped>
.about-intro-img {
  width: 900px;
  height: 350px;
  padding: 0 0 0 5vw;
  box-shadow: 3px 3px 5px grey;
  background-image: url('./../assets/DSC_0206.jpg');
  background-repeat: no-repeat;
}
</style>
