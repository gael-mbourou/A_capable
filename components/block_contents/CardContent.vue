<template>
  <b-card bg-variant="light" text-variant="dark" v-bind:title="CardTitre" class="card-hauteur">
    <b-card-text>
        {{CardContent}}
    </b-card-text>
    <b-button href="#" variant="link">{{CardTextBouton}}</b-button>
  </b-card>

</template>

<script>

export default {
  name:'CardContent',
  props:['CardTitre','CardContent','CardTextBouton']
}
</script>

<style scoped>
  .card-hauteur{
    height:280px
}
</style>


