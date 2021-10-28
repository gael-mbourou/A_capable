<template>
    <div>
        <TopNavBar></TopNavBar><br/><br/>
    </div>
</template>

<script>
import TopNavBar from '../components/bar_de_navication/TopNavBar.vue'
export default{
    name:'Recrutement',
         head() {
      // Configurer les méta tags pour cette page
      return{
        titleTemplate:"%s - récrutement",
        meta:[
          {name:"description",content:this.myDescription}
        ],
      }
    },
    data(){
      return{
        myDescription:"Récrutement facile pour toutes personnes souhaitant aider des personnes en difficulté",
      }
    },
    components:{
        TopNavBar
    }
}
</script>

<style scoped>

</style>
