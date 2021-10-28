<template>
    <div>
    <TopNavBar></TopNavBar><br/><br/>
    </div>
</template>

<script>
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
export default{
    name:'NousContacter',
         head() {
      // Configurer les méta tags pour cette page
      return{
        title:"Contacter une association d'aide pour autiste",
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
