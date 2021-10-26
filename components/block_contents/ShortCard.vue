<template>
  <div class:="shortCard">
    <b-card
      v-bind:title="CardTitre"
      v-bind:img-src="CardImageSRC"
      v-bind:img-alt="CardImageALT"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2 myshortCard"
    >
      <b-card-text>
        {{CardContent}}
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default{
  name:'ShortCard',
  props:['CardTitre','CardContent','CardImageSRC','CardImageALT'],
}
</script>

<style>
h4{
  font-size:16px;
  text-align:center;
}
.shortCard img{
  width:64px;
}
.myshortCard{
  height:250px;
}
  @media screen and (max-width: 977px) {
.myshortCard{
  height:270px;
}
}
</style>
