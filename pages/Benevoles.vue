<template>
  <div>
  <TopNavBar></TopNavBar><br/><br/><br/>
  <div class="top-bloc">
      <TextLeft v-bind:Titre="Title1" v-bind:LienImage="ImgURL" v-bind:LienBouton="LinkBtn" v-bind:SousTitre="Subtitle" v-bind:TextBouton="TextBtn" v-bind:TextAltImg="alternatifText" ></TextLeft>
    </div>

    <b-container class="bv-example-row">

        <b-row class="text-center1">
          <b-col></b-col>
          <b-col cols="5"><h2> {{Title2}} </h2></b-col>
          <b-col></b-col>
        </b-row>

        <b-row class="text-center2">
          <b-col><ShortCard v-bind:CardTitre="cardsTab[0].CardTitre2" v-bind:CardImageSRC="cardsTab[0].CardSRC"></ShortCard></b-col>
          <b-col><ShortCard v-bind:CardTitre="cardsTab[1].CardTitre2" v-bind:CardImageSRC="cardsTab[1].CardSRC"></ShortCard></b-col>
          <b-col><ShortCard v-bind:CardTitre="cardsTab[2].CardTitre2" v-bind:CardImageSRC="cardsTab[2].CardSRC"></ShortCard></b-col>
        </b-row>

      <b-row class="text-center3">
        <b-col></b-col>
        <b-col cols="9"><p class="text-justify">{{Textcontent}}</p> <p class="text-justify"> {{Textcontent2}} </p> <p class="text-justify"> {{Textcontent3}} </p>
          <h2 class="text-left">Venez nous rejoindre pour agir</h2>
          <h3 class="text-left">Nos missions :</h3>
          <ListeContent></ListeContent>
        </b-col>
        <b-col></b-col>
      </b-row>

    </b-container>
  <PiedsDePage/>
  </div>
</template>

<script>
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
import TextLeft from '../components/block_contents/TextLeft.vue'
import ShortCard from '../components/block_contents/ShortCard.vue'
import ListeContent from '../components/block_contents/ListeContent.vue'
import PiedsDePage from '../components/PiedsDePage.vue'
export default {
  name:'Benevoles',
       head() {
      // Configurer les méta tags pour cette page
      return{
        title:"Bénévoles d'association d'aide et accompagnement pour ausites",
        meta:[
          {name:"description",content:this.myDescription}
        ],
      }
    },
  data(){
    return{
      myDescription:"Les bénévoles de l'association capable sont véritablement engagé au quotidien des personnes avec trouble du spectre autistiques et personnes agées",
      cardsTab:[
        {CardTitre2:"L'amour",CardSRC:"https://gad-digital.com/wp-content/uploads/2021/10/Accueil.png"},
        {CardTitre2:"La bienveillance",CardSRC:"https://gad-digital.com/wp-content/uploads/2021/10/Presentation.png"},
        {CardTitre2:"Intégrité",CardSRC:"https://gad-digital.com/wp-content/uploads/2021/10/Evaluation.png"},
      ],

      Title2:"Ce qui nous définit",
      ImgURL:"https://gad-digital.com/wp-content/uploads/2021/09/Accompagnement-a-lexterieur-des-segnors.png",
      Title1:"Nos bénévoles s'engagent pour vous",
      Subtitle:"Ils ont choisi de vous aider à vous éppanouir dans votre quotidien",
      alternatifText:"Le bénévolat avec Association capable",
      TextBtn:"En savoir plus",
      LinkBtn:"#",

      Textcontent:"Mesdames, Messieurs, REJOIGNEZ NOUS  dans cette œuvre de bienfaisance ! Il s\’agit d\’offrir son sourire qui ne coute rien mais qui crée beaucoup confirmant l\’assertion de Marc LEV qui dit : « le sourire est une sorte de vaccin contre l\’instant de mal être » La raison d’être de notre association est de tendre une main bienveillante à ceux qui ont été fragilisé par l\’âge, la maladie ou le handicap. Il est vrai et réel que « nul de nous ne vit pour lui-même ».",

     Textcontent2:"Cette vérité biblique prouve au quotidien que tout ce que nous faisons est réalisé pour servir autrui. C\’est pourquoi, donnez un peu de votre temps ou de votre personne pour apporter  amabilité, gaité, joie, sourire à nos personnes accompagnées vous donnera en retour un sens à la vie qui est celui de porteur de bien-être.",
     Textcontent3:"Notre but dans cette lutte contre l’isolement des personnes dépendantes est d’être présent quand personne n’est là.",

    }
  },
  components:{
    TopNavBar,
    TextLeft,
    ShortCard,
    ListeContent,
    PiedsDePage,
  }
}
</script>

<style scoped>
.top-bloc{
  background-color:#364182;
}
.text-center1, .text-center3{
  margin-top:50px;
}

</style>

