<template>
   <div class="bas-de-page">
        <b-container class="bv-example-row">
            <b-row>
                <b-col sm>
                    <h5>Navigation</h5>
                    <ul>
                        <li><NuxtLink to="/">Accueil</NuxtLink></li>
                        <li><NuxtLink to="/Solutions">Solutions</NuxtLink></li>
                        <li><NuxtLink to="/Presentation">Présentation</NuxtLink></li>
                        <li><NuxtLink to="/Benevoles">Bénévoles</NuxtLink></li>
                    </ul>
                </b-col>
                <b-col sm>
                    <h5>Informations utiles</h5>
                    <ul>
                        <li><NuxtLink to="/AideFinanciere">Aide financières</NuxtLink></li>
                        <li><NuxtLink to="/Recrutements">Récrutements</NuxtLink></li>
                        <li><NuxtLink to="/Tarifs">Tarifs</NuxtLink></li>
                        <li><NuxtLink to="/NousContacter">Nous contacter</NuxtLink></li>
                    </ul>
                </b-col>
                <b-col sm> <NuxtLogo/><SocialMediaNav/> </b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
import NuxtLogo from '../components/NuxtLogo.vue'
import SocialMediaNav from '../components/block_contents/SocialMediaNav.vue'
    export default{
        name:'PiedsDePage',
        data(){
            return{

            }
        },
        components:{
            NuxtLogo,
            SocialMediaNav,
        }
    }
</script>

<style scoped>
 .bas-de-page{
     background-color:#e6d9e1;
     padding-top:50px;
 }
</style>