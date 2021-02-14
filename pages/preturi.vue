<template>
  <div class="price-container">
    <h1 class="centered-text dark-blue">Prețuri</h1>
    <ul>
      <li v-for="item in myJson" :key="item.title">
        <PriceCard :card-title="item.title" :card-content="item.content" />
      </li>
    </ul>
  </div>
</template>
<script>
import PriceCard from '~/components/PriceCard.vue'
import prices from '~/assets/data/preturi.json'
export default {
  metaInfo: {
    title: 'About us'
  },
  components: {
    PriceCard
  },
  data() {
    return {
      myJson: prices
    }
  },
  created() {
    // console.log(this.myJson)
  }
}
</script>
