<template>
  <div>
    <h3>{{ cardTitle }}</h3>
    <div v-for="item in cardContent" :key="item.service">
      <PriceItem :service="item.service" :price="item.price" />
    </div>
  </div>
</template>
<script>
import PriceItem from '~/components/PriceItem.vue'
export default {
  name: 'PriceCard',
  components: { PriceItem },
  props: {
    cardTitle: {
      type: String,
      default: ''
    },
    cardContent: {
      type: Array,
      default: null
    }
  }
}
</script>
