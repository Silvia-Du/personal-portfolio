<template>
  <div class="latest-work">
    <div class="container py-5">
      <p class="sec-title my-5">My latest work</p>
      <div class="row">
        <!-- da ciclare -->
        <div class="col-12 col-lg-4 single-work p-2">
          <div class="box debug h-100"></div>
        </div>
        <div class="col-12 col-lg-4 single-work p-2">
          <div class="box debug h-100"></div>
        </div>
        <div class="col-12 col-lg-4 single-work p-2">
          <div class="box debug h-100"></div>
        </div>
        
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LatestWork'
}
</script>

<style lang="scss" scoped >
@import '../assets/style/vars';


.latest-work{
  background-color: $bgLightGray;
  .sec-title{
    font-size: 3rem;
    font-weight: bolder;
  }

  .single-work{
    min-height: 400px;
    margin-bottom: 15px;
  }
}

</style>