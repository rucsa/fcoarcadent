<template>
  <v-app>
    <v-main>
      <NavMenu />
      <v-container class="pa-0 ma-0" fluid>
        <nuxt />
      </v-container>
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
export default {}
</script>
<style scoped>
.nav-menu-item-font {
  font-family: 'Montserrat';
  font-weight: thin;
}
.header-font {
  font-family: 'Montserrat';
  font-weight: bold;
  text-align: left;
  font: normal normal bold 50px/61px Montserrat;
  letter-spacing: 0px;
  color: #292a2a;
  opacity: 1;
}
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
/* * {
  font-family: 'Montserrat';
} */
</style>
