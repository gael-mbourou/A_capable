<template>
    <div>
  <ul class="list-unstyled">
    <b-media tag="li">
      <template #aside>
        <b-img blank blank-color="#abc" width="32" alt="placeholder"></b-img>
      </template>
      <h5 class="mt-0 mb-1">Animations culturelles </h5>
      <p class="mb-0">
        Plusieurs activités au programme avec des bénévole dynamiques et pyvalents.
      </p>
    </b-media>

    <b-media tag="li" class="my-4">
      <template #aside>
       <b-img blank blank-color="#cba" width="32" alt="placeholder"></b-img>
      </template>

      <h5 class="mt-0 mb-1"> Visites et tenir compagnie </h5>
      <p class="mb-0">
        Vous ne vous senterez plus seul dans votre quotidient.
      </p>
    </b-media>

    <b-media tag="li">
      <template #aside>
        <b-img blank blank-color="#bac" width="32" alt="placeholder"></b-img>
      </template>

      <h5 class="mt-0 mb-1"> Activités diverses </h5>
      <p class="mb-0">
        Des activités de loisirs et culturelles, des activités thématiques de toutes sortes, les activités manuelles, des jeux de mémoire, des ateliers créatifs ainsi que des ateliers de distraction.
      </p>
    </b-media>
  </ul>
</div>
</template>

<script>

export default{
    name:'ListeContent',
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