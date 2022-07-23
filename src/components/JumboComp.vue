<template>
  <div class="jumbotron debug d-flex justify-conetnt-center align-items-center">
    <div class="container">
      <div class="row">
        <div class="col col-md-6 debug text"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'JumboComp'
}
</script>

<style lang="scss" scoped >

.jumbotron{
  height: 75vh;
  margin-top: -80px;

  .text{
    min-height: 400px;
  }
}
</style>