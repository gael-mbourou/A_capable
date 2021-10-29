<template>
  <b-container class="bv-example-row">
    <b-row class="block-content ">
      <b-col  sm><ShortCard v-bind:CardTitre="cardsTab[0].CardTitre2" v-bind:CardContent="cardsTab[0].CardContent2" v-bind:CardImageSRC="cardsTab[0].CardSRC"></ShortCard></b-col>
      <b-col sm><ShortCard v-bind:CardTitre="cardsTab[1].CardTitre2" v-bind:CardContent="cardsTab[1].CardContent2" v-bind:CardImageSRC="cardsTab[1].CardSRC"></ShortCard></b-col>
      <b-col sm><ShortCard v-bind:CardTitre="cardsTab[2].CardTitre2" v-bind:CardContent="cardsTab[2].CardContent2" v-bind:CardImageSRC="cardsTab[2].CardSRC"></ShortCard></b-col>
      <b-col sm><ShortCard v-bind:CardTitre="cardsTab[3].CardTitre2" v-bind:CardContent="cardsTab[3].CardContent2" v-bind:CardImageSRC="cardsTab[3].CardSRC"></ShortCard></b-col>
      <b-col  sm><ShortCard v-bind:CardTitre="cardsTab[4].CardTitre2" v-bind:CardContent="cardsTab[4].CardContent2" v-bind:CardImageSRC="cardsTab[4].CardSRC"></ShortCard></b-col>
      <b-col sm><ShortCard v-bind:CardTitre="cardsTab[5].CardTitre2" v-bind:CardContent="cardsTab[5].CardContent2" v-bind:CardImageSRC="cardsTab[5].CardSRC"></ShortCard></b-col>
    </b-row>
  </b-container>
</template>

<script>
import ShortCard from './ShortCard.vue'
  export default{
    name:'StepBySte2',

    data(){
      return{
              cardsTab:[
        {CardTitre2:"Accueil",CardContent2:"de la personne à accompagner ",CardSRC:"Accueil.png"},
        {CardTitre2:"Présentation",CardContent2:"de l’association et de ses offres ",CardSRC:"Presentation.png"},
        {CardTitre2:"Evaluation",CardContent2:"des besoins et attentes au domicile",CardSRC:"Evaluation.png"},
        {CardTitre2:"Devis",CardContent2:"soumis à la validation de la personne à accompagner",CardSRC:"Devis.png"},
        {CardTitre2:"Contrat",CardContent2:"de prestation signé par les deux parties",CardSRC:"Contrat.png"},
        {CardTitre2:"Prise en charge",CardContent2:"de la personne à accompagner",CardSRC:"Accompagnement.png"},
      ],
      TitreH1:"Nous avons pensé à vous",
      SoutitreDuBLock:"mettre ici, une petite explication en rapport avec le titre du haut de manière cohérente "
      }
    },
    components:{
      ShortCard,
    }
  }
</script>

<style scoped>

  @media screen and (max-width: 977px) {
  .block-content{
    text-align:center;
  }
}
.tailleImage{
  height:150px;
}
.b{
display : inline-block;
}
</style>

