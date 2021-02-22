<template>
  <v-btn
    class="px-7 py-2 mx-1 my-0 button-custom"
    :style="{
      background: backgroundColor,
      fontSize: fontSize + 'px;'
    }"
    plain
    @click.stop="buttonClicked"
  >
    {{ buttonTitle }}
  </v-btn>
</template>
<script>
export default {
  name: 'Button',
  props: {
    anchor: {
      type: Boolean,
      required: false,
      default: false
    },
    buttonTitle: {
      type: String,
      default: ''
    },
    to: {
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
