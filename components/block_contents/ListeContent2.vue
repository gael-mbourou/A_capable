<template>
    <div>
  <ul class="list-unstyled">
    <b-media tag="li">
      <template #aside>
        <b-img blank blank-color="#abc" width="32" alt="placeholder"></b-img>
      </template>
      <h5 class="mt-0 mb-1">L’accompagnement des personnes avec troubles du spectre autistique </h5>
    </b-media>

    <b-media tag="li" class="my-4">
      <template #aside>
       <b-img blank blank-color="#cba" width="32" alt="placeholder"></b-img>
      </template>

      <h5 class="mt-0 mb-1"> La perte d’autonomie des personnes âgées et/ou personnes en situation de handicap </h5>
    </b-media>

    <b-media tag="li">
      <template #aside>
        <b-img blank blank-color="#bac" width="32" alt="placeholder"></b-img>
      </template>
      <h5 class="mt-0 mb-1"> L’isolement des personnes âgées et/ou personnes en situation de handicap </h5>
    </b-media>
        <b-media tag="li">
      <template #aside>
        <b-img blank blank-color="#abc" width="32" alt="placeholder"></b-img>
      </template>
      <h5 class="mt-0 mb-1"> Répit des aidants </h5>
    </b-media>
        <b-media tag="li">
      <template #aside>
        <b-img blank blank-color="#cba" width="32" alt="placeholder"></b-img>
      </template>
      <h5 class="mt-0 mb-1"> La formation des aidants </h5>
    </b-media>
  </ul>
</div>
</template>

<script>

export default{
    name:'ListeContent2',
    data(){
      return{
      
      TitleListe1:"Animations culturelles",
      TitleListe2:"Visites et tenir compagnie",
      TitleListe3:"Activités diverses: des activités de loisirs et culturelles, des activités thématiques de toutes sortes, les activités manuelles, des jeux de mémoire, des ateliers créatifs ainsi que des ateliers de distraction",

    }
  },
  props:['listeTitre1','listeTitre2','listeTitre3'],
}

<script>