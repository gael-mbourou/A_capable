<template>
  <b-container class="bv-example-row pourquoi-nous">
           <h1>{{TitreH1}}</h1>
           <p>{{SoutitreDuBLock}} </p>
            <b-row>
              <b-col >
                <CardContent :ImgSrc="cardsTab[0].LienImage" v-bind:CardTitre="cardsTab[0].CardTitre1" v-bind:CardContent="cardsTab[0].CardContent1" v-bind:CardTextBouton="CardTextBouton1"></CardContent>
              </b-col>
              <b-col >
                <CardContent :ImgSrc="cardsTab[1].LienImage" v-bind:CardTitre="cardsTab[1].CardTitre1" v-bind:CardContent="cardsTab[1].CardContent1" v-bind:CardTextBouton="CardTextBouton1"></CardContent>
              </b-col>
              <b-col >
                <CardContent :ImgSrc="cardsTab[2].LienImage" v-bind:CardTitre="cardsTab[2].CardTitre1" v-bind:CardContent="cardsTab[2].CardContent1" v-bind:CardTextBouton="CardTextBouton1"></CardContent>
              </b-col>
            </b-row>
  </b-container>
</template>

<script>
import CardContent from './block_contents/CardContent.vue'
export default {
  name:'WhyUs',
  components:{
    CardContent
  },
  data(){
    return{
      cardsTab:[
        {CardTitre1:"Personnes avec handicap",LienImage:"Aides-et-accompagnement-des-personnes-avec-handicap.png"},
        {CardTitre1:"Personnes agées",LienImage:"Aide-au-quotidien-des-parsonnes-agées.png"},
        {CardTitre1:"Personnes avec trouble du spectre autistique",LienImage:"Suivi-des-personnes-atteint-de-trouble-du-sctre-autistique.png"}
      ],
      CardTextBouton1:"découvrire  >>",
      TitreH1:"Nous avons pensé à vous",
      SoutitreDuBLock:"mettre ici, une petite explication en rapport avec le titre du haut de manière cohérente "
      
    }
  }
}
</script>

<style scoped>
.pourquoi-nous{
padding-top:80px;
padding-bottom:80px;
}
h1{
color:#ee7ae8;
}
h1,p{
text-align:center;
}

</style>

