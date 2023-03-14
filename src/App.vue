<template>
  <NavBar :logo="logo_src" :alt="app_name"/>
  <router-view/>
  <FooterVue />
</template>

<script>
import NavBar from './components/NavBar.vue'
import FooterVue from './components/FooterVue.vue';

export default {
  name: 'AppVue',
  components: {
    NavBar,
    FooterVue
  },
  data(){
    return{
      logo_src: "/img/logo.png",
      app_name: "Make your burguer"
    }
  }
}
</script>

<style>
</style>
