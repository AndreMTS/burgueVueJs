<template>
  <Navbar v-bind:logo="logo_src" v-bind:alt="app_name" />
  <RouterView />
  <Footer />
</template>

<script>

import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

export default {
  components:{
    Navbar,
    Footer
  },
  data(){
    return{
      logo_src: './img/logo.png',
      app_name: 'App Pedidos'
    }
  }
}

</script>

<style>

*{
  font-family: "Helvetica";
  padding:0;
  margin:0;
  box-sizing: border-box;
}

.main-container{
  margin:50px;
  min-height: 250px;
}
h1{
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
