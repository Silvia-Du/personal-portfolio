<template>
  <div class="jumbotron d-flex justify-conetnt-center align-items-center">
    <div class="container">
      <div class="row">
        <div class="col col-md-6 text py-5">
          <p class="name animate__animated animate__fadeInDownBig">Silvia Dugato</p>
          <p class="title animate__animated animate__fadeInDownBig">let's create responsive projects with clean and creative code.</p>
        </div>
      </div>
      <img class="me" src="../assets/img/jumboMe.png" alt="sd-img">
      <img class="form n10" src="../assets/img/10.png" alt="forms-10">
      <img class="form n5" src="../assets/img/5.png" alt="forms-5">
      <img class="form n7" src="../assets/img/7.png" alt="forms-7">
      <img class="form n3" src="../assets/img/3.png" alt="forms-3">
    </div>
  </div>
</template>

<script>
export default {
  name: 'JumboComp'
}
</script>

<style lang="scss" scoped >
@import '../assets/style/vars';
@import '../assets/style/mixin';


.jumbotron{
  padding: 130px 0;
  position: relative;
  background-color: $bgLightGray;

    img.me{
      position: absolute;
      width: 520px;
      bottom: 0;
      right: 380px;
      z-index: 870;
    }
  
    .text{
      
      .title{
        font-size: 3rem;
        font-weight: bold;
        position: relative;
        z-index: 880;
    
      }
      .name{
        font-size: 1.7rem;
        font-weight: bold;
        
        &::after{
          content: ' ';
          display: table;
          width: 60px;
          height: 1px;
          background-color: black;
          display: inline-block;
          margin: 0 0 8px 20px;  
        }
      }
    }
    img.form{
      position: absolute;
      opacity: 0.9;
    }
    .form.n10{
      width: 523px;
      transform: rotate(62deg);
      left: -16px;
      bottom: -167px;
    }
    .form.n5{
      width: 343px;
      transform: rotate(-101deg);
      bottom: -162px;
      right: -26px;
    }
    .form.n7{
      width: 200px;
      left: 0;
      top: 0;
    }
    .form.n3{
      width: 600px;
      transform: rotate(-45deg);
      top: -220px;
      right: 52px;
    }
}
</style>