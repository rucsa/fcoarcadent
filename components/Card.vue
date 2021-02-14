<template>
  <div class="card centered-text square-shadow">
    <div class="overlay">
      <h3>{{ cardTitle }}</h3>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Card',
  props: {
    imagesrc: {
      type: String,
      default: ''
    },
    icon: {
      type: String,
      default: ''
    },
    cardTitle: {
      type: String,
      default: ''
    },
    cardText: {
      type: String,
      default: ''
    }
  },
  computed: {
    image() {
      console.log('~/assets/' + this.imagesrc)
      return '~/assets/' + this.imagesrc
    }
  }
}
</script>
<style scoped>
.card {
  margin: 1em;
  height: 10em;
  width: 15em;
}

h3 {
  margin-top: 4.2em;
  color: aliceblue;
  text-shadow: 2px 2px black;
  position: relative;
  z-index: 10;
  font-family: GentiumBasic;
  font-size: 1.6em;
}

.overlay::after {
  background-color: #252663;
  content: '';
  display: block;
  position: relative;
  top: -4em;
  left: -2px;
  width: 15em;
  height: 5em;
  z-index: 1;
  opacity: 0.2;
}
</style>
