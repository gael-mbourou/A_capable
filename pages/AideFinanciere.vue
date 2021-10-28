<template>
    <div>
        <TopNavBar></TopNavBar><br/><br/>
    </div>
</template>

<script>
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
export default{
    name:'AideFinanciere',
         head() {
      // Configurer les méta tags pour cette page
      return{
        title:"Financement pour personnes avec troubles du specter autistique",
        meta:[
          {name:"description",content:this.myDescription}
        ],
      }
    },
       data(){
      return{
        myDescription:"Obtenez toutes les informations concernant les aides des proposé aux personnes avec trouble du spectre autistique ou pour personnes agées",
      }
    },
        components:{
        TopNavBar
    }
}
</script>

<style scoped>

</style>
