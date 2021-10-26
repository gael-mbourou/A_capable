<template>
  <div>
  <h2>{{TitreSection}} </h2>
  <b-container class="bv-example-row">
  <b-row class="rowclass">
    <b-col class="colonne-droite ">
      <b-nav vertical>
        <b-nav-item  v-on:click="displayContent1">{{TabTitre[0]}} </b-nav-item>
        <b-nav-item  v-on:click="displayContent2">{{TabTitre[1]}} </b-nav-item>
        <b-nav-item  v-on:click="displayContent3">{{TabTitre[2]}} </b-nav-item>
        <b-nav-item  v-on:click="displayContent4">{{TabTitre[3]}} </b-nav-item>
        <b-nav-item  v-on:click="displayContent5">{{TabTitre[4]}} </b-nav-item>
        <b-nav-item  v-on:click="displayContent6">{{TabTitre[5]}} </b-nav-item>
      </b-nav>
    </b-col>
    <b-col class="colonne-droite " cols="8">
     <b-row v-if="affiche1">
        <b-col><b-img v-bind:src="TabLinks[0]" class="tailleImage"></b-img></b-col>
        <b-col>{{TabContent[0]}}</b-col>
      </b-row>
      <b-row v-if="affiche2">
        <b-col><b-img v-bind:src="TabLinks[1]" class="tailleImage"></b-img></b-col>
        <b-col>{{TabContent[1]}}</b-col>
      </b-row>
      <b-row v-if="affiche3">
        <b-col><b-img v-bind:src="TabLinks[2]" class="tailleImage"></b-img></b-col>
        <b-col>{{TabContent[2]}}</b-col>
      </b-row>
      <b-row v-if="affiche4">
        <b-col><b-img v-bind:src="TabLinks[3]" class="tailleImage"></b-img></b-col>
        <b-col>{{TabContent[3]}}</b-col>
      </b-row>
      <b-row v-if="affiche5">
        <b-col><b-img v-bind:src="TabLinks[4]" class="tailleImage"></b-img></b-col>
        <b-col>{{TabContent[4]}}</b-col>
      </b-row>
      <b-row v-if="affiche6">
        <b-col><b-img v-bind:src="TabLinks[5]" class="tailleImage"></b-img></b-col>
        <b-col>{{TabContent[5]}}</b-col>
      </b-row>
    </b-col>
  </b-row>
  </b-container >
  </div>
</template>

<script>

export default {
  name:'StepByStep',
  data() {
    return{
      TitreSection:'Notre démarche de prise en charge',

      TabTitre:['Accueil de la personne',
        'Présentation de l\'association',
        'Evaluation des besoins',
        'Devis',
        'Contrat',
        'Prise en charge',
        ],
        TabLinks:[
          'https://gad-digital.com/wp-content/uploads/2021/09/accueil.png',
          'https://gad-digital.com/wp-content/uploads/2021/09/presentation.png',
          'https://gad-digital.com/wp-content/uploads/2021/09/learning.png',
          'https://gad-digital.com/wp-content/uploads/2021/09/invoice.png',
          'https://gad-digital.com/wp-content/uploads/2021/09/contrat.png',
          'https://gad-digital.com/wp-content/uploads/2021/09/checkmark.png'
        ],

        TabContent:[
        'contenu 1',
        'contenu 2',
        'contenu 3',
        'contenu 4',
        'contenu 5',
        'contenu 6',
        ],
        affiche1:true,
        affiche2:false,
        affiche3:false,
        affiche4:false,
        affiche5:false,
        affiche6:false,
    }
  },
  methods: {
    displayContent1: function(){
        this.affiche1=true
        this.affiche2=false
        this.affiche3=false
        this.affiche4=false
        this.affiche5=false
        this.affiche6=false
    },
        displayContent2: function(){
        this.affiche1=false
        this.affiche2=true
        this.affiche3=false
        this.affiche4=false
        this.affiche5=false
        this.affiche6=false
    },
        displayContent3: function(){
        this.affiche1=false
        this.affiche2=false
        this.affiche3=true
        this.affiche4=false
        this.affiche5=false
        this.affiche6=false
    },
        displayContent4: function(){
        this.affiche1=false
        this.affiche2=false
        this.affiche3=false
        this.affiche4=true
        this.affiche5=false
        this.affiche6=false
    },
        displayContent5: function(){
        this.affiche1=false
        this.affiche2=false
        this.affiche3=false
        this.affiche4=false
        this.affiche5=true
        this.affiche6=false
    },
        displayContent6: function(){
        this.affiche1=false
        this.affiche2=false
        this.affiche3=false
        this.affiche4=false
        this.affiche5=false
        this.affiche6=true
    }
  }
}
</script>

<style scoped>
.colonne-droite{
  padding-top:20px;
  padding-bottom:20px;
  background-color:#eeeeee;
  border-radius:10px;
  margin:5px;
}
.tailleImage{
  height:150px;
}
</style>