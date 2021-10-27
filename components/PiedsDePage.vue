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
                <b-col sm><h5>Informations utiles</h5></b-col>
                <b-col sm> <NuxtLogo/> </b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
import NuxtLogo from '../components/NuxtLogo.vue'
    export default{
        name:'PiedsDePage',
        data(){
            return{

            }
        },
        components:{
            NuxtLogo
        }
    }
</script>

<style scoped>
 .bas-de-page{
     background-color:#e6d9e1;
     padding-top:50px;
 }
</style>