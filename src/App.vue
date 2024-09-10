<script>
/* 
  Per importare ed utilizzare un componente dentro un altro devo:
  1) Importazione del componente
  2) Dichiarazione del componente
  3) Utilizzo del componente
*/

// 1) Importazione del componente
import AppHeader from './components/AppHeader.vue';

export default {
  data() {
    return{
      
    }
  },

  // 2) Dichiarazione del componente
  components: {
    AppHeader
  }
}
</script>

<template>
  <!-- 3) Utilizzo del componente -->
  <AppHeader />

</template>

<style lang="sscs" scoped>

</style>
