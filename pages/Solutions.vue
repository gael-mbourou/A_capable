<template>
  <div>
  <TopNavBar></TopNavBar>
  <div class="top-bloc">
    <TextRight v-bind:Titre="Title" v-bind:LienImage="LinkImg" v-bind:LienBouton="LinkBtn" v-bind:SousTitre="Subtitle" v-bind:TextBouton="TextBtn" v-bind:TextAltImg="alternatifText" ></TextRight>
  </div>

  <b-container class="bv-example-row accompagnement-class">
    <b-row class="text-center">
      <b-col></b-col>
      <b-col cols="9">
        <h2>{{TitreAccomagnment}} </h2>
        <p>{{ShortAccompagnement}} </p>
        <ModalBlock v-bind:TextBouton="ModalBottonText" v-bind:ModalContent="Accompagnement"></ModalBlock>
      </b-col>
      <b-col></b-col>
    </b-row>

    
  </b-container>
  <div class="demarche">
  <h2>{{DemarcheAccomagnment}} </h2><br/>
    <StepBySte2></StepBySte2>
  </div>
  <b-container class="bv-example-row padding-bloc">
  <h2>{{PersonnesAccomagnees}} </h2><br/>
    <b-row>
        <b-col sm>
          <h3>{{pad}} </h3>
          <Accordeon/>
        </b-col>
        <b-col sm>
          <h3>{{AcExt}} </h3>
          <p>{{AcExtContent}}</p>
          <h3>{{Course}} </h3>
          <p>{{CourseContent}}</p>
        </b-col>
    </b-row>
    </b-container>
    <div class="bottom-bloc">
    <TextLeft v-bind:Titre="TitreAutiste" v-bind:LienImage="LinkImgAutiste" v-bind:LienBouton="LinkBtn" v-bind:SousTitre="Subtitle" v-bind:TextBouton="TextBtn" v-bind:TextAltImg="alternatifText" ></TextLeft>
    </div>
    <PiedsDePage/>
  </div>
</template>

<script>

import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
import TextRight from '../components/block_contents/TextRight.vue'
import TextLeft from '../components/block_contents/TextLeft.vue'
import ModalBlock from '../components/block_contents/ModalBlock.vue'
import Accordeon from '../components/block_contents/Accordeon.vue'
import StepBySte2 from '../components/block_contents/StepByStep2.vue'
import PiedsDePage from '../components/PiedsDePage.vue'
export default {
  name:'Solutions',
  data(){
    return{
      ModalBottonText:'En savoir plus',

      TitreAutiste:'Personnes avec troubles du spectre autistique et/ou associés',
      AcExt:'Accompagnement à l\'extérieur',
      AcExtContent:'Le transport de la personne accompagnée est couvert par l’assurance de l’association. Il sera cependant demandé à cette dernière un remboursement des kilomètres effectués par l’intervenant.',
      Course:'Courses courantes',
      CourseContent:'La personnes accompagnée doit confier à l’intervenant à domicile la somme d’argent nécessaire, celui-ci devrait lui rendre la monnaie et les justificatifs de dépenses.',
      pad:"Aide à domicile et à la personne",
      PersonnesAccomagnees:"Personnes dépendantes",

      LinkImg:"https://gad-digital.com/wp-content/uploads/2021/09/Accomapgnement-au-quotidien-des-personnes-en-difficulte.png",
      Title :"Au quotidien des personnes avec trouble du spectre autisitique",
      Subtitle:"Service d'aide et d'accompagnement à domicile",
      TextBtn:"En savoir plus",
      LinkBtn:"https://gad-digital.com",
      alternatifText:"association capable",
      TitreAccomagnment :"Notre Accompagnement",

      ShortAccompagnement:"Notre Intervention à domicile s’appuie tout d’abord sur une approche globale de la personne accompagnée ensuite sur un principe d’ajustement continu de la prestation à ses besoins et attentes.",

      Accompagnement:"Notre Intervention à domicile s’appuie tout d’abord sur une approche globale de la personne accompagnée ensuite sur un principe d’ajustement continu de la prestation à ses besoins et attentes. En vue d’offrir en permanence un service adapté aux besoins de la personne accompagnée et/ou sa famille, l’association s’engage à procéder à une évaluation des besoins exprimés, tout en proposant  une offre élaborée conjointement avec la personne accompagnée et/ou sa famille et à assurer la coordination avec d’autres structures et/ou professionnels intervenant au domicile. De plus, elle assure ainsi la transparence de son action pour la personne accompagnée et/ou sa famille. Elle veille également à la prévention des situations de maltraitance ou des situations pouvant mettre en danger la personne accompagnée.",

      LinkImgAutiste:'https://gad-digital.com/wp-content/uploads/2021/09/Personnes-avec-troubles-du-spectre-autistique.png',
      DemarcheAccomagnment:'Une démarche qualité',
    }
  },
  components:{
    TopNavBar,
    TextRight,
    ModalBlock,
    Accordeon,
    TextLeft,
    StepBySte2,
    PiedsDePage,
  }
}
</script>

<style >
.top-bloc{
  background-color:#364182;
}
.bottom-bloc{
  background-color:#b3bcef;
}
.accompagnement-class{
  padding-top:100px;
  padding-bottom:30px;
}
h2{
  text-align:center;

}
h3{
  font-size:22px;
}
.padding-bloc{
  padding-top:80px;
  padding-bottom:80px;
}
.demarche{
  padding-top:100px;
  padding-bottom:150px;
  background-color:rgb(0 0 0 / 5%);
}
.text-center p{
  text-align: justify;
}
  @media screen and (max-width: 601px) {
h2 {
  font-size: 24px !important;
  color: #000;
}
h3{
  font-size:22px;
}

.demarche{
  padding-top:80px;
  padding-bottom:80px;
  background-color:rgb(0 0 0 / 5%);
}
}
</style>

