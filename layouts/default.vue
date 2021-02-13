<template>
  <div class="main-container">
    <NavMenu />
    <div>
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>

<script>
import NavMenu from './../components/NavMenu'
import Footer from './../components/Footer'
export default {
  components: {
    NavMenu,
    Footer
  }
}
</script>

<style lang="scss">
a {
  text-decoration: none;
  color: black;
}
a:hover {
  text-decoration: none;
  color: black;
}
.section {
  margin: 3em 0;
}
.center {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.blue {
  background-color: $blue;
}

.text-medium {
  font-weight: 400;
}

.text-bold {
  font-weight: 700;
}
.button-custom {
  font-family: 'Montserrat';
}
.flex {
  display: flex;
  flex-direction: row;
}

.flex-row {
  justify-content: space-between;
}

.flex-vertical {
  display: flex;
  flex-direction: column;
}

.main-container {
  padding: 0 120px;
}

.nav-containter {
  height: 30px;
}
</style>
