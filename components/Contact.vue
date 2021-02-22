<template>
  <div>
    <v-container
      v-if="$vuetify.breakpoint.smAndUp"
      fluid
      class="px-0 pb-16 mb-16"
    >
      <v-row class="pa-25 pb-10">
        <v-col
          cols="12"
          style="font-family: Montserrat; font-weight: bold; font-size: 20px;"
        >
          <h2 class="text-center">Contact</h2>
        </v-col>
      </v-row>
      <v-row no-gutters class="pb-10 mb-10">
        <v-col cols="8">
          <v-card flat tile style="background-color: #f2b705; height: 270px;">
            <v-card-text>
              <v-row>
                <v-col
                  class="offset-1"
                  style="font-family: Montserrat; color: #202020;"
                >
                  <h5 style="font-size: 20px; font-weight: bold;" class="pt-2">
                    Program
                  </h5>
                  <div style="font-size: 20px;">L-V:</div>
                  <div style="font-size: 18px;">10:00-17:00</div>
                  <br />
                  <h5 style="font-size: 20px; font-weight: bold;">Adresa</h5>
                  <div>str. Elocinței nr. 36, <br />Sector 1, București</div>
                  <br />
                  <h5 style="font-size: 20px; font-weight: bold;">
                    +4 0724 545 168
                  </h5>
                  <div>filofteiacoarca@yahoo.com</div>
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="4">
          <div>
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d45543.03222568537!2d26.028546045242688!3d44.48566029845745!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x902a4f4894eaa55a!2sCabinet%20Stomatologic%20dr.%20Coarc%C4%83%20Filofteia!5e0!3m2!1sen!2sro!4v1595169436264!5m2!1sen!2sro"
              height="300"
              width="100%"
              frameborder="0"
              style="border: 0;"
              allowfullscreen=""
              aria-hidden="false"
              tabindex="0"
            ></iframe>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <v-container v-if="$vuetify.breakpoint.xsOnly" class="pb-16 mb-16">
      <v-card flat tile>
        <!-- <v-row>
          <v-col class="offset-1">
            <h2>Contact</h2>
          </v-col>
        </v-row> -->
        <v-card-text>
          <v-row>
            <v-col>
              <h2 class="black--text">Contact</h2>
            </v-col>
          </v-row>
          <v-row>
            <v-col style="color: #202020;">
              <h5 class="font-weight-bold">
                Program
              </h5>
              <div>L-V:</div>
              <div>10:00-17:00</div>
              <br />
              <h5 class="font-weight-bold">Adresa:</h5>
              <div>str. Elocinței nr. 36, Sector 1, București</div>
              <h5 class="font-weight-bold">+4 0724 545 168</h5>
              <div>filofteiacoarca@yahoo.com</div>
            </v-col>
          </v-row>
          <v-row justify="center" align="center">
            <v-col>
              <div>
                <iframe
                  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d45543.03222568537!2d26.028546045242688!3d44.48566029845745!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x902a4f4894eaa55a!2sCabinet%20Stomatologic%20dr.%20Coarc%C4%83%20Filofteia!5e0!3m2!1sen!2sro!4v1595169436264!5m2!1sen!2sro"
                  frameborder="0"
                  height="300"
                  width="100%"
                  style="border: 0;"
                  allowfullscreen=""
                  aria-hidden="false"
                  tabindex="0"
                ></iframe>
              </div>
            </v-col>
          </v-row>
        </v-card-text>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  name: ''
}
</script>
<style scoped></style>
