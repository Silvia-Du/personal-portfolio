<template>
  <main>
    <JumboComp />
    <LatestWork />
    <AboutComp />
  </main>
</template>

<script>

import JumboComp from './JumboComp.vue';
import LatestWork from './LatestWork.vue';
import AboutComp from './AboutComp.vue';

export default {
  name: 'MainComp',
  components:{
    JumboComp,
    LatestWork,
    AboutComp
  }
}
</script>

<style lang="scss" scoped >

  main{
    min-height: calc(100vh - 160px);
  }

</style>