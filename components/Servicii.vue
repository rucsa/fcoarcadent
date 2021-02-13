<template>
    <div class="section servicii">
        <h1 class="center">Servicii Stomatologice</h1>
        <div class="card-container">
            <Card class="profilaxie" cardTitle='PROFILAXIE' cardText='cardtext1'/>
            <Card class="estetica-dentara" cardTitle='ESTETICA DENTARA' cardText='cardtext1'/>
            <Card class="endodontie" cardTitle='ENDODONTIE' cardText='cardtext1'/>
            <Card class="proteica" cardTitle='PROTETICA' cardText='cardtext1'/>
            <Card class="chirurgie-dentara" cardTitle='CHIRURGIE  DENTARA' cardText='cardtext1'/>
            <Card class="parodontologie" cardTitle='PARODONTOLOGIE' cardText='cardtext1'/>
            <Card class="ortodontie" cardTitle='ORTODONTIE' cardText='cardtext1'/>
        </div>
     
  </div>
</template>
<script>
import Button from './../components/Button'
import Card from './../components/Card'

export default {
    name: 'Servicii'
    
}
</script>
<style scoped>
.card-container {
    padding: 0px 15em;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}
.profilaxie {
  background-image: url('./../assets/profilaxie.png');
  background-size: contain;
  background-repeat:no-repeat;
}
.estetica-dentara {
  background-image: url('./../assets/estetica.png');
  background-size: contain;
  background-repeat:no-repeat;
}
.endodontie {
  background-image: url('./../assets/Endodontie.png');
  background-size: contain;
  background-repeat:no-repeat;
}
.proteica {
  background-image: url('./../assets/protetica.png');
  background-size: contain;
  background-repeat:no-repeat;
}
.chirurgie-dentara {
  background-image: url('./../assets/chirurgie-dentara.png');
  background-size: contain;
  background-repeat:no-repeat;
}
.parodontologie {
  background-image: url('./../assets/parodontologie.png');
  background-size: contain;
  background-repeat:no-repeat;
}
.ortodontie {
  background-image: url('./../assets/ortodontie.png');
  background-size: contain;
  background-repeat:no-repeat;
}
</style>