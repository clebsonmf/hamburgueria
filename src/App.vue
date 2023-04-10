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
*{
  box-sizing: border-box;
  font-family: Helvetica;
  margin: 0;
  padding: 0;
}

.main-container{
  margin: 50px;
  min-height: 250px;
}
h1{
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
