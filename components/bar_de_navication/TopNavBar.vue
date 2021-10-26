<template>
  <b-navbar toggleable="lg" type="dark" variant="light" class="navbar-fixed-top">
    <b-navbar-brand href="#"><NuxtLogo/></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item><nuxt-link to="/">Accueil</nuxt-link></b-nav-item>
        <b-nav-item><nuxt-link to="/Solutions">Nos solutions</nuxt-link></b-nav-item>
        <b-nav-item><nuxt-link to="/Presentation">Présentation</nuxt-link></b-nav-item>
        <b-nav-item><nuxt-link to="/Benevoles">Bénévoles</nuxt-link></b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
/*import {b-nav-item,b-navbar-nav,b-collapse,b-navbar} from 'bootstrap-vue',*/
export default{
  name:'TopNavBar',
  components:{
   /* b-nav-item,
    b-navbar-nav,
    b-collapse,
    b-navbar*/
  }
}
</script>

<style>
      .navbar-toggler {
    padding: 0.25rem 0.75rem;
    font-size: 1.25rem;
    line-height: 1;
    background-color: #dc3545;
    border: 1px solid transparent;
    border-radius: 0.25rem;
}
li a{
font-size:18px;
color:#000;
}
.navbar-fixed-top{
  position:fixed;
  width:100%;
  z-index:1000;
  box-shadow: rgba(0, 0, 0, 0.15) 0px 1px 15px;
}
</style>