<template>
  <div>
    <TopNavBar></TopNavBar>
    <div class="top-bloc">
      <TextLeft v-bind:Titre="Title1" v-bind:LienImage="LinkImg" v-bind:LienBouton="LinkBtn" v-bind:SousTitre="Subtitle" v-bind:TextBouton="TextBtn" v-bind:TextAltImg="alternatifText" ></TextLeft>
    </div>
  <b-container class="bv-example-row pt-5 bloc2">
  <h2>{{Title2}}</h2><br/>
    <b-row>
      <b-col></b-col>
      <b-col cols="9">{{Right}}
      </b-col>
      <b-col></b-col>
    </b-row>
    </b-container>
    <div class="bgc-bloc3 bloc3">
      <b-container class="bv-example-row pt-5">
      <div>
      <h2 > {{Title3}} </h2>
      <b-row>
        <b-col ><br/><br/>
          <ListeContent2/>
        </b-col>
        <b-col><b-img :src="LinkImg2" fluid-grow alt="Fluid-grow image"></b-img></b-col>
      </b-row>
      </div>
      </b-container>
    </div>

    <b-container class="bv-example-row pt-1">
    <div class="bloc4">
    <h2> {{Title4}} </h2>
    <b-row >
      <b-col><b-img :src="LinkImg3" fluid-grow alt="Fluid-grow image"></b-img></b-col>
      <b-col><p>{{bloccontent4}}</p><br/> <p>{{bloccontent5}}</p> </b-col>
    </b-row>
    </div>
  </b-container><br/><br/><br/>
  <PiedsDePage/>
  </div>

</template>

<script>
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
import TextLeft from '../components/block_contents/TextLeft.vue'
import PiedsDePage from '../components/PiedsDePage.vue'
import ListeContent2 from '../components/block_contents/ListeContent2.vue'
export default {
  name:'Presentation',
       head() {
      // Configurer les méta tags pour cette page
      return{
        title:"Ptésentation d'une Association pour autistes et personnes agées",
         meta:[
          {name:"description",content:this.myDescription}
        ],
      }
    },
  data(){
    return{
      myDescription:"Association capable est une association lois 1901 qui aide et accompagne accompagne au quotidien des personnes avec trouble du spectre autistique et personnes agées",
      LinkImg:"Suivi-des-personnes-havec-handicape.png",
      Title1 :"Nous contribuons à redonner espoire",
      Subtitle:"Service d'aide et d'accompagnement à domicile",
      TextBtn:"En savoir plus",
      LinkBtn:"https://gad-digital.com",
      alternatifText:"Aide de personnes en difficulté",
      LinkImg2:"Aide-à-domicile-pour-personnes-agées.png",
      Title2 :"Qui sommes-nous ?",
      Title3 :"Pourquoi nous solliciter ?",
      Title4 :"Notre battement de coeur",
      LinkImg3:"https://cdn.pixabay.com/photo/2021/08/21/12/08/impossible-6562613_960_720.jpg",

      Right:"L’association Capable SAAD est une structure à but non lucratif loi 1901, crée en 2018 pour répondre aux besoins croissants d’aide à domicile des personnes dépendantes dans le cadre du maintien à domicile des personnes âgées et des personnes en situation de handicap, et de celui de l’accompagnement à domicile des personnes avec Troubles du spectre autistique (TSA) et/ou associés.L’association Capable SAAD a été créée sur l’initiative d’un groupe d’amis, composé médecin, infirmière, éducateurs spécialisés, aide médico-sociale qui exerce dans le médico-social, mené par Madame NDOMBI MAMBUANA Séverine. Dans notre vocation d’agir en faveur d’autrui, l’association CAPABLE SAAD veut apporter sa contribution pour répondre à la problématique de :",

      bloccontent4:"L’association CAPABLE SAAD met au centre de son action, l’aspect humain qui consiste à apporter aux personnes accompagnées la gaité, la joie, la confiance en soi, l’empathie… en un mot apporter grâce ses bénévoles et salariés un grand sourire, dont l’objectif est de restaurer la relation avec l’autre quand plus personne n’est là et d’amener la joie de vivre.",

      bloccontent5:"Un sourire ne coute rien mais il crée beaucoup. C’est le sens que nous donnons à notre action qu’on retrouve dans la citation de Marc LEVY : « le sourire est une sorte de vaccin contre l’instant de mal être ».",
    }
  },
  components:{
    TopNavBar,
    TextLeft,
    PiedsDePage,
    ListeContent2
  }
}
</script>

<style scoped>
.top-bloc{
background-color:#364182;
}
.bloc2, .bloc3, .bloc4{
  margin-top:50px;
  margin-bottom:50px;
}
.bgc-bloc3{
  background-color:#e3e5f2;
  padding-top:0px;
  padding-bottom:80px;
}
</style>

