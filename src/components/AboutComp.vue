<template>
  <div class="debug">
    <div class="container">
      
      <div class="about debug">about</div>
      <!-- servizi -->
      <div class="services debug py-5">
        <div class="container-fluid py-5">
          <div class="row">
            <div class="col-12 col-md-6 debug serv-col"> servizi, 4 con icona e descrizione</div>
            <div class="col-12 col-md-6 debug serv-col">testo sopa grosso sotto piccolo</div>
          </div>
        </div>
      </div>
      <!-- linguaggi -->
      <div class="dev-language debug">Linguaggi lista</div>
    </div>
  </div>
  
</template>

<script>
export default {
  name: 'AboutComp'
}
</script>

<style lang="scss" scoped >

.about{
  min-height: 500px;
}

.services{
  min-height: 300px;
  .serv-col{
    min-height: 400px;
  }
}

.dev-language{
  min-height: 300px;
}


</style>