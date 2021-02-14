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
    <div>
      <div class="despre-servicii">
        <div class="card-container flex">
          <IconCard
            imagesrc="~/assets/icons/1.png"
            card-text="Profesionalismul si dedicatia personalului medical"
          />
          <IconCard
            imagesrc="~/assets/icons/2.png"
            card-text="Aparatura medicala stomatologica de ultima generatie"
          />
          <IconCard
            imagesrc="~/assets/icons/3.png"
            card-text="Tehnici medicale stomatologice inovatoare"
          />
          <IconCard
            imagesrc="~/assets/icons/4.png"
            card-text="Adresabilitate maxima corespunzatoare cerințelor pacienților"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import IconCard from '~/components/IconCard.vue'
export default {
  name: 'About',
  components: {
    IconCard
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
      specialtext: 'Apreciată de micii pacienti'
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
}
</style>
