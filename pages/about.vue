<template>
  <div class="container">
    <div class="about-intro flex">
      <div class="about-intro-text">
        <p>Medic titular: {{ name }}</p>
        <p>Grad medical: {{ grad }}</p>
        <p>Experiență: {{ experienta }}</p>
        <p>Perfecționare profesională: {{ perfectionare }}</p>
        <p>Atitudine: {{ atitudine }}</p>
        <h3 class="special-text">{{ specialtext }}</h3>
      </div>
      <div class="about-intro-img"></div>
    </div>
    <div v-if="showSpecs">
      <div class="despre-servicii">
        <h1 class="centered-text">
          Calitatea serviciilor noastre stomatologice este un mix intre:
        </h1>
      </div>
      <div class="card-container flex">
        <Card
          icon="true"
          imagesrc="icon-professional.jpg"
          card-text="Profesionalismul si dedicatia personalului medical"
        />
        <Card
          card-title="ICON"
          card-text="Aparatura medicala stomatologica de ultima generatie"
        />
        <Card
          card-title="ICON"
          card-text="Tehnici medicale stomatologice inovatoare"
        />
        <Card
          card-title="ICON"
          card-text="Adresabilitate maxima corespunzatoare cerințelor pacienților"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Card from '~/components/Card.vue'
export default {
  name: 'About',
  components: {
    Card
  },
  data() {
    return {
      name: 'Coarcă Filofteia',
      grad: 'Medic stomatolog specialist',
      experienta:
        '33 ani vechime și peste 10.000 de pacienți tratati cu succes',
      perfectionare:
        'Continuă prin participare la congrese, simpozioane, workshopuri, cursuri de perfecționare în stomatologie',
      atitudine: 'Hotărîre, perseverență, apropiat și înțelegător cu pacienții',
      specialtext: 'Apreciată de micii pacienti',
      showSpecs: false
    }
  },
  computed: {
    owner() {
      return {
        name: 'Filofteia Coarca'
      }
    }
  },
  methods: {}
}
</script>

<style scoped>
.about-intro {
  width: 100%;
}
.about-intro-img {
  width: 900px;
  height: 350px;
  padding: 0 0 0 5vw;
  box-shadow: 3px 3px 5px grey;
  background-image: url('./../assets/DSC_0206.jpg');
  background-repeat: no-repeat;
}
.about-intro-text {
  padding: 5vh 5vw;
}
.card-container {
  justify-content: space-between;
}</style
>s
