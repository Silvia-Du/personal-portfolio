<template>
  <div id="app">

    <HeaderComp />
    <MainComp />
    <FooterComp />
    
  </div>
</template>

<script>

import HeaderComp from './components/partials/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/partials/FooterComp.vue';

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  }
}
</script>

<style lang="scss">

</style>
