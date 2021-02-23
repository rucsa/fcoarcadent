<template>
  <v-btn
    v-if="!hasAnchor"
    class="px-7 py-2 mx-1 my-0 button-custom"
    :style="{
      background: backgroundColor,
      fontSize: fontSize + 'px;'
    }"
    plain
    @click.stop="buttonClicked"
    >{{ buttonTitle }}
  </v-btn>
  <v-btn
    v-else
    class="px-7 py-2 mx-1 my-0 button-custom"
    :style="{
      background: backgroundColor,
      fontSize: fontSize + 'px;'
    }"
    plain
  >
    <nuxt-link :to="to" color="black"> {{ buttonTitle }}</nuxt-link>
  </v-btn>
</template>
<script>
export default {
  name: 'Button',
  props: {
    anchor: {
      type: String,
      required: false,
      default: ''
    },
    hasAnchor: {
      type: Boolean,
      required: false,
      default: false
    },
    buttonTitle: {
      type: String,
      default: ''
    },
    path: {
      type: String,
      default: ''
    },
    fontSize: {
      type: Number,
      default: 30
    },
    fontWeigth: {
      type: Number,
      default: 800
    },
    backgroundColor: {
      type: String,
      default: '#f2b705'
    }
  },
  computed: {
    to() {
      return this.hasAnchor ? { path: this.path, hash: this.anchor } : this.path
    }
  },
  methods: {
    buttonClicked(event) {
      this.$emit('clicked', event)
    }
  }
}
</script>
<style scoped>
.button-custom {
  font-family: 'Montserrat';
  font-weight: 800;
  color: black;
  border-radius: 25px;
  opacity: 1;
}

a {
  text-decoration: none;
}
</style>
