<template>
  <div class="cover container-fluid">
    <Cover />
    <DespreComponent />
    <Servicii />
    <Contact />
  </div>
</template>

<script>
import Cover from './../components/Cover'
import Servicii from './../components/Servicii'
import Contact from './../components/Contact'
import DespreComponent from './../components/DespreComponent'

export default {
  components: {
    Cover, DespreComponent, Servicii, Contact
  },
  data() {
    return {
      title: 'Cabinet Stomatologic dr. Filofteia Coarca'
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

<style lang="scss">


</style>
