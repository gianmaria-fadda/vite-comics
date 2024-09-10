<script>
/* 
  Per importare ed utilizzare un componente dentro un altro devo:
  1) Importazione del componente
  2) Dichiarazione del componente
  3) Utilizzo del componente
*/

// 1) Importazione del componente
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return{
      
    }
  },

  // 2) Dichiarazione del componente
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <!-- 3) Utilizzo del componente -->
  <AppHeader />
  <AppMain />
  <AppFooter />

</template>

<style lang="sscs" scoped>

</style>
