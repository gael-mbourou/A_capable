<template>
  <div>
    <TopNavBar></TopNavBar>
    <div class="fdcolor">
          <TextLeft v-bind:Titre="Title1" v-bind:LienImage="LinkImg1" v-bind:LienBouton="LinkBtn1" v-bind:SousTitre="Subtitle1" v-bind:TextBouton="TextBtn1" v-bind:TextAltImg="alternatifText1" ></TextLeft>
    </div>
    
    <WhyUs></WhyUs>

    <div class="about-association-capable">
          <TextRight v-bind:Titre="Title2" v-bind:LienImage="LinkImg2" v-bind:LienBouton="LinkBtn2" v-bind:SousTitre="Subtitle2" v-bind:TextBouton="TextBtn2" v-bind:TextAltImg="alternatifText2" ></TextRight>
    </div>
  </div>
</template>

<script>
import Tutorial from '../components/Tutorial.vue'
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
import TextLeft from '../components/block_contents/TextLeft.vue'
import TextRight from '../components/block_contents/TextRight.vue'
import WhyUs from '../components/WhyUs.vue'
export default {
  name:'index',
  data(){
    return{
      LinkImg1:"https://gad-digital.com/wp-content/uploads/2021/09/Aide-et-accompagnement-des-autistes.png",
      Title1 :"Au quotidien des personnes avec trouble du spectre autisitique",
      Subtitle1:"Service d'aide et d'accompagnement à domicile",
      TextBtn1:"En savoir plus",
      LinkBtn1:"https://gad-digital.com",
      alternatifText1:"association capable",
      
      LinkBtn2:"https://gad-digital.com",
      TextBtn2:"En savoir plus",
      Title2 :"Le rôle de l'association capable au service des personnes en difficulté",
      Subtitle2:"que vous soyez une personne agée, une personne avec handicap ou que vous présentez des troubles du spectre autistique, nous vous proposons des solutions adaptées à votre besoin.",
      LinkImg2:"https://gad-digital.com/wp-content/uploads/2021/09/Accompagnement-des-personnes-agees.png",
      alternatifText2:"association capable"
    }
  },
  components:{
   Tutorial,
   TopNavBar,
   TextLeft,
   TextRight,
   WhyUs,
  }
}
</script>

<style>
  .fdcolor{
    background-color:#ee7ae8;
  }
  p{
    font-size:18px;
    padding-top:10px;
  }
  h1{
    font-size:40px !important;
    color:#000;
  }
  h1,p{
    text-align: left;
  }

  .about-association-capable{
        background-color:#ee7ae8;
        text-align:center;
    }
</style>
