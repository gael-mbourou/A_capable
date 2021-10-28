<template>
    <div>
    <TopNavBar></TopNavBar><br/><br/>
    </div>
</template>

<script>
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
export default{
    name:'Tarifs',
         head() {
      // Configurer les méta tags pour cette page
      return{
        title:"Tarifs pour pour accompagnement des personnes avec trouble autistique",
        meta:[
          {name:"description",content:this.myDescription}
        ],
      }
    },
    data(){
      return{
        myDescription:"Association capable mets à votre disposition des tarifs adaptés à vos besoins. ces tarifs sont fonction de votre situation et nous vous conseillons pour l'obtension des aides",
      }
    },
     components:{
        TopNavBar
    }
}
</script>

<style scoped>

</style>

