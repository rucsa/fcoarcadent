<template>
  <v-container class="my-5">
    <h2
      class="pl-5 pt-5"
      style="
        color: #202020;
        font-family: Montserrat;
        font-weight: bold;
        font-size: 20px;
      "
    >
      Prețuri
    </h2>
    <v-expansion-panels tile flat class="mb-16 pb-16">
      <v-expansion-panel v-for="item in myJson" :key="item.title">
        <v-expansion-panel-header
          class="mt-5 subtitle-2"
          color="#F2B705"
          expand-icon="mdi-plus"
          >{{ item.title }}</v-expansion-panel-header
        >
        <v-expansion-panel-content
          v-for="x in item.content"
          :key="x.service"
          color="#F2F2F2"
        >
          <v-row>
            <v-col cols="6">
              <div class="mt-5">
                {{ x.service }}
              </div>
            </v-col>
            <v-col cols="6">
              <div class="mt-5" style="text-align: end;">
                {{ x.price }}
              </div>
            </v-col>
          </v-row>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-container>
  <!-- <div class="">
    <h1 class="">Prețuri</h1>
    <ul>
      <li v-for="item in myJson" :key="item.title">
        <PriceCard :card-title="item.title" :card-content="item.content" />
      </li>
    </ul>
  </div> -->
</template>
<script>
import prices from '~/assets/data/preturi.json'
export default {
  metaInfo: {
    title: 'About us'
  },
  data() {
    return {
      myJson: prices
    }
  }
}
</script>
