<template>
  <div >
    <b-container class="bv-example-row">
      <b-row>
        <b-col class="texte-left" sm>
          <h1>{{Titre}}</h1>
          <p>{{SousTitre}}</p>
          <b-button variant="outline-primary" v-bind:href="LienBouton">{{TextBouton}}</b-button>
        </b-col>
        <b-col sm>
          <b-img v-bind:src="LienImage" fluid v-bind:alt="TextAltImg" right></b-img>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>


export default {
  name:'TextLeft',
  data(){
    return{
      
    }
  },
  props:['Titre','SousTitre','LienBouton','TextBouton','LienImage','TextAltImg'],
}
</script>

<style scoped>
.texte-left{
  padding-top: 150px;
  padding-bottom: 80px;
}
  @media screen and (max-width: 601px) {
.texte-left{
  padding-top: 50px;
  padding-bottom: 50px;
}
h1 {
    font-size: 26px !important;
    color: #000;
}
}
</style>