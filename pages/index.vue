<template>
  <v-container fluid class="pa-0 ma-0">
    <div class="text-center">
      <v-dialog v-model="dialog" width="700px" heigth="651px">
        <v-card>
          <v-img :src="dialogImage">
            <v-row>
              <v-col cols="11">
                <div
                  class="mt-15"
                  style="
                    background-color: #05aff2;
                    font-family: Ananda;
                    border-top-right-radius: 5px;
                    border-bottom-right-radius: 5px;
                  "
                >
                  <p
                    class="text-center text-md-h4 font-weight-bold white--text pt-2 pb-2"
                  >
                    Luptăm împreună împotriva virusului!
                  </p>
                </div>
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="4" class="pb-0">
                <div
                  class="mt-5 pr-2"
                  style="
                    background-color: #05aff2;
                    font-family: Ananda;
                    text-align: end;
                    border-top-right-radius: 5px;
                    border-bottom-right-radius: 5px;
                  "
                >
                  <p
                    class="white--text pb-1 pt-1 pr-2 text-md-h5 font-weight-bold"
                  >
                    Ne-am vaccinat!
                  </p>
                </div>
              </v-col>
            </v-row>
            <v-row class="mt-0">
              <v-col cols="12" md="6">
                <div class="ml-5 pl-3 pr-2">
                  <p
                    style="
                      color: #05aff2;
                      font-family: Ananda;
                      text-align: start;
                      font-size: 25px;
                    "
                    class="font-weight-bold p-5 pt-1"
                  >
                    Si ne luăm <br />
                    în continuare <br />
                    toate măsurile <br /><span
                      style="
                        color: #f2b705;
                        background-color: white;
                        border-top-right-radius: 5px;
                        border-bottom-right-radius: 5px;
                      "
                      class="pt-1 pb-1 pr-2"
                      >sanitare necesare.</span
                    >
                  </p>
                </div>
              </v-col>
            </v-row>
            <v-card-actions>
              <v-spacer></v-spacer>
              <Button button-title="Am ințeles" @clicked="buttonClicked" />
              <v-spacer></v-spacer>
            </v-card-actions>
          </v-img>
        </v-card>
      </v-dialog>
    </div>
    <Cover />
    <DespreComponent />
    <Servicii />
    <Contact />
  </v-container>
</template>

<script>
import image from '~/assets/img/Dr_small.png'
export default {
  data() {
    return {
      title: 'Cabinet Stomatologic dr. Filofteia Coarca',
      dialog: false,
      dialogImage: image
    }
  },
  created() {
    if (process.browser && !sessionStorage.getItem('hasSeenDialog') === true) {
      this.showOpeningDialog()
    }
  },
  methods: {
    showOpeningDialog() {
      sessionStorage.setItem('hasSeenDialog', true)
      this.dialog = true
    },
    buttonClicked(event) {
      this.dialog = false
    }
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: 'fcoarcadent',
          name: 'Cabinet Stomatologic dr. Filofteia Coarca',
          content: 'Cabinet Stomatologic situat in Sector 1 Bucuresti'
        }
      ]
    }
  }
}
</script>
