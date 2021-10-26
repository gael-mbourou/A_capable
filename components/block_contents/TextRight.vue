<template>
  <div >
    <b-container class="bv-example-row">
      <b-row>
        <b-col sm>
          <b-img v-bind:src="LienImage" fluid v-bind:alt="TextAltImg" left></b-img>
        </b-col>
        <b-col class="texte-right" sm>    
          <h1>{{Titre}}</h1>
          <p>{{SousTitre}}</p>
          <b-button variant="outline-primary" v-bind:href="LienBouton">{{TextBouton}}</b-button>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>


export default {
  name:'TextRight',
  data(){
    return{
      
    }
  },
  props:['Titre','SousTitre','LienBouton','TextBouton','LienImage','TextAltImg'],
}
</script>

<style scoped>
@media screen and (min-width: 601px) {
  .texte-right{
    padding-top: 150px;
    padding-bottom: 80px;
  }
}
 @media screen and (max-width: 601px) {
  .texte-right{
    padding-bottom: 10px;
  }
  .texte-right h1{
    font-size: 26px !important;
  }
}
</style>