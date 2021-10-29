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

<style>
  .card-hauteur{
    height:280px
}
.card-title {
    margin-bottom: 0.75rem;
    font-weight: bolder;
}
.card-text{
  font-size:14px;
  text-align:center;
}
.card-body {
    flex: 1 1 auto;
    min-height: 1px;
    padding: 0.25rem;
        padding-top: 0.25rem;
        padding-right: 0.25rem;
        padding-bottom: 0.25rem;
        padding-left: 0.25rem;
}
.card {
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-color: #fff;
    background-clip: border-box;
    border: 1px solid rgba(255, 255, 255, 0.13);
    border-radius: 0.25rem;
}
</style>


