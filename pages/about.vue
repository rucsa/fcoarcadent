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
              style="color: #05aff2; font-family: Ananda; font-size: 25px;"
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
          :src="require(`~/assets/img/DSC_0206.JPG`)"
        ></v-img>
      </v-col>
    </v-row>
    <v-row justify="center" align="center" class="mt-8 pb-16 mb-16">
      <v-col cols="12" sm="4" md="3" lg="3">
        <IconCard
          icon-number="1"
          card-text="Profesionalismul și dedicația personalului medical"
        />
      </v-col>
      <v-col cols="12" sm="4" md="3" lg="3">
        <IconCard
          icon-number="2"
          card-text="Aparatură medicală stomatologică de ultimă generație"
        />
      </v-col>
      <v-col cols="12" sm="4" md="3" lg="3">
        <IconCard
          icon-number="3"
          card-text="Tehnici medicale stomatologice inovatoare"
        />
      </v-col>
      <v-col cols="12" sm="4" md="3" lg="3">
        <IconCard
          icon-number="4"
          card-text="Adresabilitate maximă corespunzătoare cerințelor pacienților"
        />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      name: 'Coarcă Filofteia',
      grad: 'Medic stomatolog specialist',
      experienta:
        '33 ani vechime și peste 10.000 de pacienți tratați cu succes',
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

<style scoped></style>
