<template>
  <v-card class="mx-auto" color="#2f99ee" width="250" height="250">
    <v-card-text>
      <v-img
        class="mt-2"
        style="display: block; margin-left: auto; margin-right: auto;"
        width="50"
        height="50"
        :src="require(`./../assets/icons/${iconNumber}.png`)"
      ></v-img>
      <p class="text-center white--text mt-4" style="font-size: 1rem;">
        Adresabilitate maximă corespunzătoare cerințelor pacienților
      </p>
    </v-card-text>
  </v-card>
</template>
<script>
export default {
  name: 'IconCard',
  props: {
    iconNumber: {
      type: String,
      default: ''
    },
    cardText: {
      type: String,
      default: ''
    }
  }
}
</script>
<style scoped></style>
